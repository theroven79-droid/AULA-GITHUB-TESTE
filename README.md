# Aula GitHub — Exercícios de C++

Repositório com três programas de terminal que praticam entrada de dados, condicionais e funções em C++. As atividades executáveis estão na pasta [Atividade](Atividade/README.md).

## Conteúdo

| Arquivo | Objetivo e regra implementada |
|---|---|
| [exercicio_01.cpp](Atividade/exercicio_01.cpp) | Lê uma idade inteira: abaixo de 18 exibe “Menor de idade.”; a partir de 18, “Maior de idade.” |
| [exercicio_02.cpp](Atividade/exercicio_02.cpp) | Lê um inteiro e usa uma função com ponteiro para verificar o intervalo inclusivo de 10 a 20. |
| [exercicio_03.cpp](Atividade/exercicio_03.cpp) | Lê um `float` e o classifica como positivo, negativo ou zero usando uma função que recebe o valor. |
| [teste_codigo.cpp](teste_codigo.cpp) | Contém somente o comentário `//teste`; não possui `main`. |
| [teste.txt](teste.txt) | Arquivo vazio. |

A pasta de atividades também guarda executáveis `.exe`. O código-fonte é a referência para o comportamento descrito aqui.

## Compilar e executar

Com um compilador `g++` disponível, execute da raiz:

```bash
mkdir -p /tmp/aula-github-teste
g++ -std=c++17 Atividade/exercicio_01.cpp -o /tmp/aula-github-teste/idade
/tmp/aula-github-teste/idade
```

Cada arquivo da pasta `Atividade` possui seu próprio `main` e deve ser compilado separadamente. Os exemplos usam apenas `iostream` e `locale.h`, sem dependências de terceiros.

## Exemplos para conferir as condições

| Programa | Entrada | Resultado esperado pelo código |
|---|---|---|
| Exercício 01 | `17` | Menor de idade |
| Exercício 01 | `18` | Maior de idade |
| Exercício 02 | `10` ou `20` | Dentro do intervalo |
| Exercício 02 | `9` ou `21` | Fora do intervalo |
| Exercício 03 | `2.5`, `-2.5` ou `0` | Positivo, negativo ou zero, respectivamente |

## Observações

Os programas chamam `setlocale(LC_ALL, "portuguese")`; a disponibilidade dessa localidade depende da máquina. Alguns textos dos fontes têm caracteres acentuados em codificação diferente de UTF-8, o que pode afetar a exibição no terminal. Não há validação explícita para entrada não numérica nem suíte de testes automatizados.

Consulte o [guia das atividades](Atividade/README.md) para compilar os outros exercícios.
