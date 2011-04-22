__lojaexemploazure__

Exemplo de como desenvolver aplicativos para Windows Azure.

Prop�sito
=========

Uma simula��o de loja virtual para compras pela Internet.

Casos de uso
============

Explorar cat�logo
-----------------

O usu�rio seleciona uma categoria; o aplicativo exibe a lista de itens pertencentes � categoria.

Consultar item
--------------

O usu�rio clica sobre um item da lista de items; o aplicativo exibe detalhes do item selecionado.

Colocar na sacola
-----------------

Na consulta de um item, o usu�rio clica o bot�o "Colocar na sacola"; o aplicativo adiciona o item � sacola de compras e exibe a sacola de compras.

Consultar sacola de compras
---------------------------

O usu�rio clica no link da sacola de compras; o aplicativo exibe os itens inclu�dos na sacola de compras.

* Alternativa: O usu�rio clica no bot�o "Retirar da sacola" associado a um item; o aplicativo remove o item da sacola de compras e exibe a sacola de compras atualizada.

Comprar
-------

Na consulta da sacola de compras, o usu�rio clica o bot�o "Comprar"; o aplicativo pede os dados necess�rios e registra o pedido.

Acompanhar pedido
-----------------

O usu�rio clica sobre o link "Acompanhar pedidos"; o aplicativo apresenta a lista de pedidos do usu�rio com a sua respectiva situa��o.

* Alternativa: O usu�rio clica sobre um pedido da lista; o aplicativo apresenta os detalhes do pedido incluindo dados de cobran�a, itens e valor total.

Arquitetura
===========

O aplicativo possui uma arquitetura modular:

![Arquitetura](doc/Arquitetura.png)

* _Frente de Loja_: Interface web utilizada pelos consumidores finais.
* _�rea administrativa_: Interface web utilizada pelos administradores da loja.
* _Servi�o da Loja_: Web service que exp�e uma interface padronizada para a l�gica de neg�cio e acesso a dados do aplicativo.
* _Processamento da Loja_: Servi�o de processamento de tarefas em segundo plano e integra��o com back office.
