# GenstageExample

In this example we’ll be constructing a GenStage application that emits numbers, 

sorts out the even numbers, and finally prints them.

For our application we’ll use all three GenStage roles. Our producer will be responsible for counting and emitting numbers. We’ll use a producer-consumer to filter out only the even numbers and later respond to demand from downstream. Last we’ll build a consumer to display the remaining numbers for us.
[GenStarge Elixir School](https://elixirschool.com/en/lessons/advanced/gen-stage/)

## To Run

```
$ mix do deps.get, compile
$ mix run --no-halt
```

## Casos de uso

Agora que cobrimos o GenStage e construímos nossa primeira aplicação exemplo, quais são alguns casos de uso reais do GenStage?

- **Pipeline de Transformação de Dados** — Produtores não precisam ser simples geradores de números. Poderíamos produzir eventos de um banco de dados ou mesmo de outra fonte como Apache Kafka. Com uma combinação de produtor-consumidores e consumidores, podemos processar, ordenar, catalogar, e armazenar métricas à medida que elas ficam disponíveis.

- **Filas de Trabalho** — Uma vez que eventos podem ser qualquer coisa, poderíamos produzir unidades de trabalho para serem completadas por uma séries de consumidores.

- **Processamento de Eventos** — Semelhante a um pipeline de dados, poderíamos receber, processar, classificar e agir em eventos emitidos em tempo real de nossas fontes.

Estas são apenas algumas possibilidades para o GenStage.

