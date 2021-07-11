# 3.4 Operadores Aritméticos

Assim como toda a linguagem de programação o Bash também suporta alguns operadores aritméticos. Eles são os operadores de adição, subtração, multiplicação, divisão, módulo (resto da divisão) e exponenciação.

Em Bash, existe duas formas de utilizar esses comandos, usando `expr` e `$((Operador))`. Como veremos um pouco melhor ao passar por cada operador.

## Operador de Adição

Como o nome já diz, é um operador que realiza uma soma, ele pode ser atribuido dentro de variáveis ou realizando soma de duas variáveis, no exemplo abaixo fará mais sentido.

```bash
#! /bin/bash

echo `expr 3 + 2`
echo $((3+2))
```

## Operador de subtração

Como o nome já diz, é um operador que realiza uma subtração, ele pode ser atribuido dentro de variáveis ou realizando subtrações de duas variáveis, no exemplo abaixo fará mais sentido.

```bash
#! /bin/bash

echo `expr 3 - 2`
echo $((3-2))
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

## Operador de multiplicação

Como o nome já diz, é um operador que realiza uma multiplicação, ele pode ser atribuido dentro de variáveis ou realizando multiplicações de duas variáveis, no exemplo abaixo fará mais sentido.

```bash
#! /bin/bash

echo `expr 3 \* 2`
echo $((3*2))
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

## Operador de divisão

Como o nome já diz, é um operador que realiza uma divisão, ele pode ser atribuido dentro de variáveis ou realizando divisões de duas variáveis, no exemplo abaixo fará mais sentido.

```bash
#! /bin/bash

echo `expr 4 / 2`
echo $((4 / 2))
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

## Operador de Módulo

Esse operador retorna o resto de uma divisão. O exemplo abaixo fica mais simples de entender.

```bash
#! /bin/bash

echo `expr 3 % 2`
echo $((3 % 2))
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

## Operador de Exponenciação

Esse operador retorna a potência de um número com o expoênte dado, como podemos observar mais abaixo.

```bash
#! /bin/bash

echo $((3**2))
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!


<p align="center">
  <a href="03-Entrada-e-saída.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="05-Operadores-lógicos.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>