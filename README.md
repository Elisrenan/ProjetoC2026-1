````markdown
# Avaliação Prática — Lógica de Programação em C

## Conteúdos Avaliados

- Tabela verdade com operadores lógicos `&&` (AND) e `||` (OR)
- Condicionais com `if`, `else if` e `else`
- Estruturas de repetição (`for`, `while` e `do while`)
- Vetores simples para armazenamento de dados

---

# Questão 1 — Controle de Aprovação de Participantes

## Contexto

Um curso de programação deseja analisar o desempenho de **8 participantes**.

Para cada participante, o sistema deverá ler:

- Nota final
- Frequência em percentual

As notas deverão ser armazenadas em um vetor.

---

## Parte A — Tabela Verdade

Considere as proposições:

```text
p = nota >= 7
q = frequencia >= 75
````

A regra de aprovação é:

```text
Aprovado = p && q
```

Complete a tabela verdade:

| p | q | p && q |
| - | - | ------ |
| V | V |        |
| V | F |        |
| F | V |        |
| F | F |        |

---

## Parte B — Regra de Negócio

O participante será classificado da seguinte forma:

* Se `nota >= 7` **e** `frequencia >= 75`, exibir `APROVADO`
* Caso contrário, exibir `REPROVADO`

Ao final, o programa deverá mostrar:

* Quantidade de aprovados
* Quantidade de reprovados
* Maior nota registrada

---

## Código Base

```c
#include <stdio.h>

int main() {
    float notas[8];
    float frequencia;
    int i;

    int aprovados = 0;
    int reprovados = 0;

    float maiorNota = 0;

    // Implemente aqui:
    // 1. Ler as 8 notas e armazenar no vetor notas
    // 2. Ler a frequência de cada participante
    // 3. Usar if com AND para classificar
    // 4. Contar aprovados e reprovados
    // 5. Descobrir a maior nota

    return 0;
}
```

---

# Questão 2 — Análise de Vendas Simples

## Contexto

Uma pequena loja deseja analisar as vendas realizadas em um dia.

O sistema deverá registrar o valor de **10 vendas** em um vetor.

---

## Parte A — Tabela Verdade

Considere as proposições:

```text
p = valorVenda >= 100
q = vendaEspecial == 1
```

A regra de destaque é:

```text
Destaque = p || q
```

Complete a tabela verdade:

| p | q | p || q |
|---|---|--------|
| V | V |        |
| V | F |        |
| F | V |        |
| F | F |        |

---

## Parte B — Regra de Negócio

Para cada venda, leia:

* Valor da venda
* Indicador se a venda foi especial (`1` para sim, `0` para não)

A venda será classificada assim:

* Se `valorVenda >= 100` **ou** `vendaEspecial == 1`, exibir `VENDA COM DESTAQUE`
* Caso contrário, exibir `VENDA COMUM`

Ao final, o programa deverá mostrar:

* Total vendido
* Quantidade de vendas com destaque
* Quantidade de vendas comuns

---

## Código Base

```c
#include <stdio.h>

int main() {
    float vendas[10];
    int vendaEspecial;
    int i;

    float totalVendido = 0;
    int destaque = 0;
    int comum = 0;

    // Implemente aqui:
    // 1. Ler as 10 vendas e armazenar no vetor vendas
    // 2. Ler se cada venda foi especial
    // 3. Usar if com OR para classificar
    // 4. Somar o total vendido
    // 5. Contar vendas com destaque e comuns

    return 0;
}
```

---

# Questão 3 — Controle de Temperaturas Simples

## Contexto

Um laboratório precisa registrar **7 medições de temperatura** realizadas ao longo do dia.

As temperaturas deverão ser armazenadas em um vetor.

---

## Parte A — Tabela Verdade

Considere as proposições:

```text
p = temperatura >= 20
q = temperatura <= 30
```

A temperatura é considerada segura quando:

```text
Segura = p && q
```

Complete a tabela verdade:

| p | q | p && q |
| - | - | ------ |
| V | V |        |
| V | F |        |
| F | V |        |
| F | F |        |

---

## Parte B — Regra de Negócio

Para cada temperatura:

* Se `temperatura >= 20` **e** `temperatura <= 30`, exibir `TEMPERATURA SEGURA`
* Caso contrário, exibir `TEMPERATURA FORA DA FAIXA`

Ao final, o programa deverá mostrar:

* Quantidade de temperaturas seguras
* Quantidade de temperaturas fora da faixa
* Média das temperaturas

---

## Código Base

```c
#include <stdio.h>

int main() {
    float temperaturas[7];
    int i;

    int seguras = 0;
    int foraFaixa = 0;

    float soma = 0;
    float media;

    // Implemente aqui:
    // 1. Ler as 7 temperaturas e armazenar no vetor temperaturas
    // 2. Usar if com AND para verificar a faixa segura
    // 3. Contar temperaturas seguras e fora da faixa
    // 4. Calcular a média

    return 0;
}
```

---

# Critérios de Correção

| Critério                               | Pontuação |
| -------------------------------------- | --------: |
| Tabelas verdade corretas               |       2,0 |
| Uso correto de vetores                 |       2,0 |
| Uso correto de loops                   |       2,0 |
| Uso correto de condicionais com AND/OR |       2,0 |
| Exibição correta dos resultados        |       2,0 |
| **Total**                              |  **10,0** |

---

# Instruções ao Aluno

1. Complete as tabelas verdade.
2. Analise cuidadosamente as regras de negócio.
3. Implemente a lógica dentro do código base fornecido.
4. Teste seu programa com diferentes valores.
5. Entregue o código-fonte de cada questão.

```
```
