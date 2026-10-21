# Atividade — Condicionais e funções em C++

[Voltar ao README principal](../README.md)

Esta pasta reúne três exercícios independentes. Cada arquivo `.cpp` contém sua própria função `main` e tem um executável `.exe` correspondente no repositório.

## Conteúdo dos exercícios

| Arquivo | O que o programa faz | Conceitos presentes |
|---|---|---|
| [exercicio_01.cpp](exercicio_01.cpp) | Lê uma idade inteira e compara o valor com 18. | Entrada com `cin`, saída com `cout` e `if/else`. |
| [exercicio_02.cpp](exercicio_02.cpp) | Verifica se um inteiro está no intervalo inclusivo de 10 a 20. | Função `resultado(int *n)`, ponteiro e operador lógico `&&`. |
| [exercicio_03.cpp](exercicio_03.cpp) | Classifica um número como positivo, negativo ou zero. | Tipo `float`, função com passagem por valor e `if/else if/else`. |

## Compilar

Execute os comandos abaixo a partir da raiz do repositório, em um terminal Bash com `g++` disponível:

```bash
mkdir -p /tmp/aula-github-teste
g++ Atividade/exercicio_01.cpp -o /tmp/aula-github-teste/idade
g++ Atividade/exercicio_02.cpp -o /tmp/aula-github-teste/intervalo
g++ Atividade/exercicio_03.cpp -o /tmp/aula-github-teste/sinal
```

## Executar e conferir

Escolha um dos executáveis:

```bash
/tmp/aula-github-teste/idade
/tmp/aula-github-teste/intervalo
/tmp/aula-github-teste/sinal
```

Cada programa solicita um número e termina após apresentar o resultado.

| Exercício | Entradas de exemplo | Classificações correspondentes |
|---|---|---|
| Idade | `17` e `18` | Menor de idade e maior de idade. |
| Intervalo | `9`, `10`, `20` e `21` | Fora, dentro, dentro e fora do intervalo. |
| Sinal | `5`, `-5` e `0` | Positivo, negativo e zero. |

Os comandos de compilação usam os fontes e preservam os arquivos `.exe` já existentes na pasta.
