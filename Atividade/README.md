# Atividades — Condicionais e funções

[Voltar ao repositório](../README.md)

## O que cada exercício demonstra

- [Exercício 01](exercicio_01.cpp): compara uma idade inteira com 18 usando `if/else`.
- [Exercício 02](exercicio_02.cpp): passa o endereço de um inteiro para `resultado(int *n)`; a função verifica `*n >= 10 && *n <= 20`.
- [Exercício 03](exercicio_03.cpp): passa um `float` por valor para `resultado(float n)`; a função diferencia valores maiores que zero, menores que zero e iguais a zero.

## Compilação independente

A partir da raiz do repositório:

```bash
mkdir -p /tmp/aula-github-teste
g++ -std=c++17 Atividade/exercicio_01.cpp -o /tmp/aula-github-teste/idade
g++ -std=c++17 Atividade/exercicio_02.cpp -o /tmp/aula-github-teste/intervalo
g++ -std=c++17 Atividade/exercicio_03.cpp -o /tmp/aula-github-teste/sinal
```

Execute o binário desejado e informe um número:

```bash
/tmp/aula-github-teste/intervalo
```

Use 10 e 20 para verificar os limites inclusivos; 9 e 21 ficam fora do intervalo. No exercício de idade, 18 já entra em “Maior de idade”. No exercício de sinal, 0 tem uma saída própria.

Os `.exe` desta pasta são artefatos já compilados. Os comandos acima geram novos executáveis a partir dos fontes, sem substituir esses arquivos.
