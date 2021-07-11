# 3.3 Entrada e Saída

Para você observar alguns resultados de operações feitas em bash ou receber entradas de usuários, precisamos utilizar funções padrões (echo ou printf e read).

## Echo

A função `echo` repete o que você diz para repetir (realmente como se fosse eco).

Esta função, diferente de algumas linguagens, pode imprimir qualquer tipo, ou até mesmo ser chamada sem parámetro nenhum, imprimindo assim uma linha vazia.

### Exemplo:

```bash
#! /bin/bash

echo "Testando 1, 2, 3"

```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

É importante ressaltar que não é necessário utilizar as aspas duplas quando você utiliza esta função, contudo, para evitar problemas com aspas simples ou também aspas duplas é recomendado utilizar.

Caso seja necessário, ainda assim, utilizar algum caractere como aspas simples ou aspas duplas dentro da saída, é necessário utilizar `\` antes de cada aspa a ser impressa no terminal.

## Printf

A função `printf` é exatamente similar ao printf do C. Portanto, tambem é necessário passar o formato do argumento na string a ser impressa e posteriormente os parâmetros, como podemos ver melhor abaixo:

### Exemplo:

```bash
#! /bin/bash

printf "Número de vagas Vazias: %s" "34"
printf "Número de vagas Ocupadas: %s" "16"
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

## Read

A função `read` para a execução do programa até o usuário escrever um argumento. Após o usuário escrever o argumento, esse resultado (por padrão) será armazenado em uma variável de nome REPLY, como podemos ver melhor abaixo:

### Exemplo:

```bash
#! /bin/bash

echo "Qual o seu Nome?"
read
echo "Olá, ${REPLY}. Seja bem-vindo ao curso de Bash"
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

Porém, caso não queira salvar o output do reply na variável `REPLY`, é possível adicionar um parâmetro que será o nome da variável que a entrada será armazenada, como podemos ver melhor abaixo:

### Exemplo:

```bash
#! /bin/bash

echo "Qual o seu Nome?"
read NAME
echo "Olá, ${NAME}. Seja bem-vindo ao curso de Bash"
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

<p align="center">
  <a href="02-Declaração-de-variáveis.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="04-Operadores-aritméticos.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>