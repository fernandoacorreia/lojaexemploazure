__lojaexemploazure__

Exemplo de como desenvolver aplicativos para Windows Azure.

Copyright (C) 2011, Fernando de Alcântara Correia <fernandoacorreia@gmail.com>.

Propósito
=========

Uma simulação de loja virtual para compras pela Internet.

Casos de uso
============

Explorar catálogo
-----------------

O usuário seleciona uma categoria; o aplicativo exibe a lista de itens pertencentes à categoria.

Consultar item
--------------

O usuário clica sobre um item da lista de items; o aplicativo exibe detalhes do item selecionado.

Colocar na sacola
-----------------

Na consulta de um item, o usuário clica o botão "Colocar na sacola"; o aplicativo adiciona o item à sacola de compras e exibe a sacola de compras.

Consultar sacola de compras
---------------------------

O usuário clica no link da sacola de compras; o aplicativo exibe os itens incluídos na sacola de compras.

* Alternativa: O usuário clica no botão "Retirar da sacola" associado a um item; o aplicativo remove o item da sacola de compras e exibe a sacola de compras atualizada.

Comprar
-------

Na consulta da sacola de compras, o usuário clica o botão "Comprar"; o aplicativo pede os dados necessários e registra o pedido.

Acompanhar pedido
-----------------

O usuário clica sobre o link "Acompanhar pedidos"; o aplicativo apresenta a lista de pedidos do usuário com a sua respectiva situação.

* Alternativa: O usuário clica sobre um pedido da lista; o aplicativo apresenta os detalhes do pedido incluindo dados de cobrança, itens e valor total.

Arquitetura
===========

O aplicativo possui uma arquitetura modular:

![Arquitetura](lojaexemploazure/raw/master/doc/Arquitetura.png)

* _Frente de Loja_: Interface web utilizada pelos consumidores finais.
* _Área administrativa_: Interface web utilizada pelos administradores da loja.
* _Serviço da Loja_: Web service que expõe uma interface padronizada para a lógica de negócio e acesso a dados do aplicativo.
* _Processamento da Loja_: Serviço de processamento de tarefas em segundo plano e integração com back office.
