#DESAFIO ITAUTECH - FORMULÁRIO DE CADASTRO PESSOAL

##DESCRIÇÃO
Buscou-se desenvolver um formulário simples para cadastro, que receba principais dados (nome, CPF, RG, endereço etc.) requisitos estabelecidos
previamente pela organização do projeto.

- Tecnologias empregadas:HTML, Javascript e CSS;
- Objetivo:demonstrar aprendizado de conceitos aprendidos ao longo de duas semanas de bootcamp ministrado pela Gama Academy em conjunto com o Itaú;
- Autor:Leandro Alcolumbre.


###Estrutura dos arquivos

- HTML:

Contêm as principais funcionalidades. Formulário com container a modo de estrutura principal e separado em 5 grupos menores, ajustando-se dados de acordo com
sua afinidade. Botão de submeter do formulário vinculado a método do script JS que realiza o alerta de envio de dados se satisfeitas condições e
preenchimentos. Ademais, há integração com script para realizar validação do CEP e, se for inserido no campo respectivo, poderá haver preenchimento
automático dos demais campos do endereço.

Dois campos foram adicionados com o objetivo de saber do usuário se tem alguma deficiência. Em caso positivo, se requere, de forma opcional, que a
descreva em um campo de edição. Optou-se desta forma já que a Lei Brasileira de Inclusão (lei nº 13.146/2015) e outras normas trazem extenso rol e,
por isso mesmo, acreditou-se mais didático dar liberdade ao usuário para descrevê-la em uma cadeia de caracteres.

Buscando-se atender as determinações da Lei Geral de Proteção de Dados (lei no 13.709/2018) adicionou-se, no final, checkbox para confirmar
consentimento no compartilhamento de dados.

Por fim, além do container, semanticamente colocou-se o rodapé em uma tag footer, para fins meramente estruturais.


- Javascript

O script está dividido em duas partes principais. A primeira encontra-se no método carregaEndereco(), que recebe o cep inserido no formulário,
verifica se possui 8 números e, por fim, submete-o ao site viacep.com.br para obtenção automática do endereço. Tal se dá por meio de um objeto JSON e,
após isso, preenche os campos com os dados retornados pelo referido site. Se houver erro, informará o usuário por meio de um alert.

A segunda parte do JS é o método sucesso(), que é chamado pelo botão que submete o formulário. É informado, então, que os dados foram preenchidos e
enviados com sucesso.


- CSS

Por mais que não seja um requisito obrigatório para pessoas cegas, optou-se por utilizar este recurso como meio de tornar a página melhor estruturada
visualmente para que não haja problemas de visualização por pessoas que não fazem uso de leitores de tela.
