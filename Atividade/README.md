# 📘 Atividades — Estruturas condicionais e funções

[← Página inicial do repositório](../README.md)

Esta pasta reúne **três exercícios independentes em C++**. Cada um lê um valor pelo terminal, avalia uma condição e mostra o resultado correspondente.

## 📂 Arquivos e conceitos

| Arquivo | Entrada | Regra utilizada |
|---|---|---|
| [`exercicio_01.cpp`](exercicio_01.cpp) | Número inteiro (idade) | Idade menor que 18: menor de idade; caso contrário: maior de idade. |
| [`exercicio_02.cpp`](exercicio_02.cpp) | Número inteiro | Verifica se o valor está entre 10 e 20, inclusive. |
| [`exercicio_03.cpp`](exercicio_03.cpp) | Número decimal (`float`) | Diferencia números positivos, negativos e iguais a zero. |

O exercício 02 utiliza uma função que recebe um ponteiro (`int *`), enquanto o exercício 03 recebe uma cópia do valor (`float`).

## ⚙️ Compilar

Com `g++` instalado, execute os comandos abaixo na raiz do repositório:

```bash
g++ Atividade/exercicio_01.cpp -o idade
g++ Atividade/exercicio_02.cpp -o intervalo
g++ Atividade/exercicio_03.cpp -o sinal
```

Em Linux/macOS, execute o exercício desejado com `./idade`, `./intervalo` ou `./sinal`. Em Windows, execute o arquivo `.exe` correspondente.

## 🧪 Casos de teste manuais

| Exercício | Entradas de exemplo | Resultados esperados |
|---|---|---|
| Idade | `17`, `18` | Menor de idade; maior de idade |
| Intervalo | `9`, `10`, `20`, `21` | Fora; dentro; dentro; fora |
| Sinal | `-3`, `0`, `3` | Negativo; zero; positivo |

## 💡 O que observar no código

No exercício de intervalo, a expressão `resultado(&n)` passa o **endereço** da variável para a função, que utiliza `*n` para ler seu conteúdo. No exercício de sinal, `resultado(n)` passa o **valor** de `n`.

Os programas não salvam dados em arquivos nem tratam explicitamente entradas não numéricas. Os executáveis `.exe` já presentes são artefatos compilados, não substitutos dos códigos-fonte.
