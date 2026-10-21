# 🧩 Exercícios de programação em C++

Repositório acadêmico com três programas independentes para praticar **entrada de dados, estruturas condicionais, funções e passagem de parâmetros**. Cada exercício possui seu próprio arquivo `.cpp` e pode ser executado no terminal.

## 📚 Exercícios disponíveis

| Exercício | Objetivo | Conceitos utilizados | Código |
|---|---|---|---|
| 01 — Maioridade | Identificar se uma idade é menor ou maior ou igual a 18 anos. | `if/else`, `cin` e `cout` | [`exercicio_01.cpp`](Atividade/exercicio_01.cpp) |
| 02 — Intervalo | Verificar se um inteiro pertence ao intervalo de 10 a 20, incluindo os limites. | Ponteiros, função `void` e operador `&&` | [`exercicio_02.cpp`](Atividade/exercicio_02.cpp) |
| 03 — Sinal numérico | Classificar um valor como positivo, negativo ou zero. | `float`, `if/else if/else` | [`exercicio_03.cpp`](Atividade/exercicio_03.cpp) |

O arquivo [`Atividade/README.md`](Atividade/README.md) apresenta explicações e casos de teste de cada programa.

## 📂 Organização

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

A pasta `Atividade/` também contém os executáveis `.exe` já compilados. O arquivo `teste_codigo.cpp` não possui função `main`, e `teste.txt` está vazio.

## ⚙️ Compilação e execução

**Pré-requisito:** compilador `g++` instalado. Na raiz do repositório:

```bash
g++ Atividade/exercicio_01.cpp -o idade
g++ Atividade/exercicio_02.cpp -o intervalo
g++ Atividade/exercicio_03.cpp -o sinal
```

Em Linux ou macOS, execute `./idade`, `./intervalo` ou `./sinal`. No Windows, utilize os arquivos `.exe` gerados.

**Importante:** cada exercício possui uma função `main`; portanto, compile os arquivos separadamente.

## ✅ Exemplos para conferir

| Programa | Entrada | Classificação esperada |
|---|---|---|
| Maioridade | `17` / `18` | Menor de idade / maior de idade |
| Intervalo | `9` / `10` / `20` / `21` | Fora / dentro / dentro / fora |
| Sinal | `-2` / `0` / `2` | Negativo / zero / positivo |

Os resultados são determinados pelas condições presentes nos códigos, não por uma suíte automatizada de testes.

## 🔎 Observações técnicas

- Os programas utilizam `locale.h` e `setlocale`; a apresentação dos acentos pode variar conforme o terminal.
- Não há tratamento específico para entradas não numéricas.
- No exercício 02, `resultado(&n)` envia o endereço de uma variável; no exercício 03, `resultado(n)` passa o valor diretamente.

**[Acessar o guia detalhado dos três exercícios →](Atividade/README.md)**
