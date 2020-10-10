# Modelo de Entidade-Relacionamento (ME-R)
O Modelo de Entidade-Relacionamento (ME-R) é baseado na percepção do mundo real que consiste em um conjunto de objetos básicos chamados **Entidades** e nos **Relacionamentos** entre estes objetos. o ME-R foi desenvolvido para facilitar o projeto de banco de dados, permitindo a especificação de um esquema de "negócio", onde tal esquema representa a estrutura lógica geral do Banco de Dados (BD).

## Entidade
* Conjunto de objetos da realidade modelada sobre os quais deseja-se colecionar dados no banco de dados;
* Pode ser concreta ou abstrata;
* Uma entidade representa um conjunto de objetos que se deseja guardar dados e é importante para o seu mundo real.
* Geralmente substantivo escrito totalmente em maiúsculo;
* **Exemplo:** em um sistema bancário, as entidades podem ser clientes, contas correntes, cheques, agências, entre outros.

## Relacionamentos
* Um conjunto de relacionamentos é uma coleção de ocorrências das entidades relacionadas (associadas);
* Verbo significativo ao relacionamento existente entre as entidades participantes (representa o que ocorre no mundo real).

## Atributos
* Dado que é associado a cada ocorrência de uma entidade ou um relacionamento
* Uma Entidade é representada por um único ou vários atributos;
* O atributo mapeia uma entidade em um domínio.

## Chave
É um ou mais atributos que permitem identificar unicamente uma entidade no conjunto de registros da entidade.

* **Chave Candidata** é o atributo, ou a composição de mais que um atributo, que pode identificar unicamente uma entidade.
* **Chave Primária** define a chave candidata escolhida pelo projetista de dados para identificar unicamente os registros em uma entidade.

## Cardinalidade
É uma restrição de mapeamento que expressa o número de entidades as quais outra entidade pode ser associada via um conjunto de relacionamentos.

* Um pra um (**1:1**)
* Um pra muitos (**1:n**)
* Muitos pra um (**n:1**)
* Muitos pra muitos (**n:m**)

# **Estrutura Geral de um ME-R**
**ENTIDADES**

* Entidade1
* Entidade2
* Entidade3

**ATRIBUTOS**

* Entidade 1 (<u>atributoChavePrimária</u>, atributo2, atributoComposto(atributoComp1, atributoComp2), {atributo_multivalorado})
* Entidade 2 (<u>atributoChavePrimária</u>, atributo2)
* Entidade 3 (<u>atributoChavePrimária</u>, atributo2)

**RELACIONAMENTOS**

ENTIDADE1 - **verbo** - ENTIDADE2

* A ENTIDADE1 ... verbo ... ENTIDADE2, e a ENTIDADE2 ... verbo ... ENTIDADE1.
* Cardinalidade: **1:1, 1:n, n:1 ou n:m**
