# Aula GitHub Teste

Repositório com exercícios de C++ para praticar entrada de dados, estruturas condicionais e funções. Os três programas estão na pasta [Atividade](Atividade/README.md).

## Organização

| Caminho | Conteúdo |
|---|---|
| [Atividade](Atividade/README.md) | Três exercícios com código-fonte e executáveis `.exe`. |
| [teste_codigo.cpp](teste_codigo.cpp) | Arquivo de teste que contém apenas o comentário `//teste`. |
| [teste.txt](teste.txt) | Arquivo vazio. |

## Exercícios

| Código-fonte | Entrada | Regra aplicada |
|---|---|---|
| [exercicio_01.cpp](Atividade/exercicio_01.cpp) | Uma idade inteira | Idades menores que 18 são classificadas como “Menor de idade.”; as demais, como “Maior de idade.” |
| [exercicio_02.cpp](Atividade/exercicio_02.cpp) | Um número inteiro | Verifica se o número pertence ao intervalo de 10 a 20, incluindo os dois limites. A função recebe um ponteiro para o número. |
| [exercicio_03.cpp](Atividade/exercicio_03.cpp) | Um número do tipo `float` | Informa se o número é positivo, negativo ou zero. A função recebe o número por valor. |

## Compilação e execução

Cada exercício tem sua própria função `main` e deve ser compilado separadamente. Com `g++` disponível, execute os comandos abaixo na raiz do repositório, em um terminal Bash:

```bash
mkdir -p /tmp/aula-github-teste
g++ Atividade/exercicio_01.cpp -o /tmp/aula-github-teste/idade
/tmp/aula-github-teste/idade
```

Digite uma idade quando o programa solicitar. Por exemplo, `17` resulta em “Menor de idade” e `18` resulta em “Maior de idade”.

Os comandos geram o executável fora da pasta do repositório. Consulte o [guia da pasta Atividade](Atividade/README.md) para compilar os três programas.

## Observações sobre os fontes

Os programas incluem `iostream` e `locale.h` e chamam `setlocale(LC_ALL, "portuguese")`. A exibição dos acentos depende da codificação dos arquivos e da configuração do terminal.

O arquivo `teste_codigo.cpp` não tem uma função `main`; portanto, não é um quarto exercício executável.
