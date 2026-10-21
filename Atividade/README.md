# 📘 Atividades — condicionais e funções

[← Voltar ao repositório](../README.md)

Três exercícios independentes de programação em C++. Cada fonte possui `main()` e recebe entradas pelo terminal.

## Exercícios

| Arquivo | Entrada | Condição central | Técnica |
|---|---|---|---|
| [exercicio_01.cpp](exercicio_01.cpp) | Idade inteira | `idade < 18` | `if/else` |
| [exercicio_02.cpp](exercicio_02.cpp) | Inteiro | `*n >= 10 && *n <= 20` | Ponteiro e função `void` |
| [exercicio_03.cpp](exercicio_03.cpp) | Decimal (`float`) | `n > 0`, `n < 0` ou `0` | Parâmetro por valor |

## ⚙️ Compilar separadamente

Na raiz do repositório, com `g++` disponível:

```bash
g++ Atividade/exercicio_01.cpp -o idade
g++ Atividade/exercicio_02.cpp -o intervalo
g++ Atividade/exercicio_03.cpp -o sinal
```

Cada comando gera **um** programa; não compile os três fontes juntos.

## 🧪 Casos de teste manuais

| Cenário | Entrada | Resultado conforme o código |
|---|---:|---|
| Idade abaixo do limite | `17` | Menor de idade |
| Idade no limite | `18` | Maior de idade |
| Antes do intervalo | `9` | Fora |
| Limite inferior | `10` | Dentro |
| Limite superior | `20` | Dentro |
| Depois do intervalo | `21` | Fora |
| Número negativo | `-3` | Negativo |
| Número neutro | `0` | Zero |
| Número positivo | `3` | Positivo |

## 💡 Conceitos fundamentais

**Ponteiro:** no exercício 02, `resultado(&n)` envia o endereço da variável; a função acessa seu valor com `*n`. **Passagem por valor:** no exercício 03, `resultado(n)` recebe uma cópia do número. Em ambos, a classificação é exibida com `cout`.

## 📌 Limitações

Os programas não persistem dados, não oferecem testes automatizados e não têm tratamento específico para entradas não numéricas. Os arquivos `.exe` presentes na pasta são artefatos compilados; para estudar a implementação, utilize os `.cpp`.
