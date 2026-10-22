# 📘 Relatório da pasta — Atividade

[← Relatório do repositório](../README.md)

## 📌 Resumo

A pasta contém **três exercícios de C++**, voltados ao estudo das estruturas condicionais e da utilização de funções. Cada programa lê um dado informado pelo usuário, aplica uma condição e apresenta o resultado no terminal.

## 📂 Arquivos analisados

| Código-fonte | Finalidade | Conceitos |
|---|---|---|
| [`exercicio_01.cpp`](exercicio_01.cpp) | Distinguir idades menores e maiores ou iguais a 18 anos. | `cin`, `cout` e `if/else`. |
| [`exercicio_02.cpp`](exercicio_02.cpp) | Conferir se um número inteiro está entre 10 e 20, inclusive. | Função `void`, ponteiro e operador `&&`. |
| [`exercicio_03.cpp`](exercicio_03.cpp) | Identificar números positivos, negativos e iguais a zero. | Tipo `float` e `if/else if/else`. |

Também há três executáveis Windows, [`exercicio_01.exe`](exercicio_01.exe), [`exercicio_02.exe`](exercicio_02.exe) e [`exercicio_03.exe`](exercicio_03.exe), correspondentes aos exercícios.

## 🧠 Análise do conteúdo

No primeiro programa, a condição `idade < 18` determina a classificação. No segundo, a função `resultado` recebe o endereço de um inteiro e avalia os limites do intervalo. No terceiro, a função recebe um valor `float` e realiza três possíveis classificações.

| Entrada de referência | Comportamento previsto |
|---|---|
| Idade `17` ou `18` | Menor de idade ou maior de idade, respectivamente. |
| Inteiros `9`, `10`, `20` e `21` | Fora, dentro, dentro e fora do intervalo. |
| Valores `-3`, `0` e `3` | Negativo, zero e positivo. |

## 🔎 Considerações

Os três programas são independentes, não possuem armazenamento persistente e não tratam explicitamente entradas inválidas. Para estudar as condições e as funções, recomenda-se consultar os arquivos-fonte; os resultados da tabela são exemplos baseados no código, não uma suíte de testes automatizados.
