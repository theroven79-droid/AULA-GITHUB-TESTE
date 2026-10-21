# 🧩 Fundamentos de programação — exercícios em C++

Repositório acadêmico com três exercícios independentes de **entrada e saída, estruturas condicionais, funções e ponteiros**. Os exemplos foram escritos em arquivos `.cpp` e podem ser compilados separadamente com `g++`.

[![C++](https://img.shields.io/badge/Linguagem-C%2B%2B-00599C?logo=cplusplus&logoColor=white)](https://isocpp.org/) [![GitHub](https://img.shields.io/badge/Plataforma-GitHub-181717?logo=github)](https://github.com/theroven79-droid/AULA-GITHUB-TESTE)

## 📌 Visão geral

| Exercício | Conceito | Comportamento | Código |
|---|---|---|---|
| 01 — Maioridade | `if/else` | Classifica idades menores que 18 como menores de idade. | [exercicio_01.cpp](Atividade/exercicio_01.cpp) |
| 02 — Intervalo | Ponteiro e `&&` | Verifica se um número está no intervalo **inclusivo** de 10 a 20. | [exercicio_02.cpp](Atividade/exercicio_02.cpp) |
| 03 — Sinal | `float` e `else if` | Identifica número positivo, negativo ou igual a zero. | [exercicio_03.cpp](Atividade/exercicio_03.cpp) |

Os programas usam `cin`, `cout`, `locale.h` e `setlocale`. O resultado é apresentado no terminal, sem persistência em arquivos ou banco de dados.

## 📂 Estrutura

```text
AULA-GITHUB-TESTE/
├── Atividade/
│   ├── README.md
│   ├── exercicio_01.cpp
│   ├── exercicio_02.cpp
│   └── exercicio_03.cpp
├── README.md
├── teste_codigo.cpp
└── teste.txt
```

A pasta `Atividade` também contém executáveis `.exe`. `teste_codigo.cpp` é somente um arquivo de teste, sem `main`, e `teste.txt` está vazio.

## ⚙️ Compilação e execução

**Pré-requisito:** `g++` instalado e disponível no terminal. Na raiz do repositório:

```bash
g++ Atividade/exercicio_01.cpp -o idade
g++ Atividade/exercicio_02.cpp -o intervalo
g++ Atividade/exercicio_03.cpp -o sinal
```

No Linux/macOS, execute `./idade`, `./intervalo` ou `./sinal`. No Windows, use os nomes de saída com `.exe` e execute-os no terminal. Cada `.cpp` possui sua própria função `main`, portanto os arquivos não devem ser vinculados como um único programa.

## ✅ Exemplos para conferir

| Programa | Entrada | Resultado esperado |
|---|---:|---|
| Maioridade | `17` / `18` | Menor / maior de idade |
| Intervalo | `9` / `10` / `20` / `21` | Fora / dentro / dentro / fora |
| Sinal | `-2` / `0` / `2` | Negativo / zero / positivo |

Os exemplos correspondem às condições presentes no código; não representam testes automatizados.

**📖 Documentação detalhada:** [guia da pasta Atividade](Atividade/README.md).

## 🔎 Notas técnicas

- A codificação e o terminal podem influenciar a exibição de acentos após `setlocale`.
- Os exercícios não tratam explicitamente entradas não numéricas.
- Para compreender o uso de ponteiros, compare `resultado(&n)` no exercício 02 com `resultado(n)` no exercício 03.
