# 3.5 Operadores lógicos e de Comparação

Os operadores lógicos são utilizados quando é necessário usar duas ou mais condições dentro da mesma instrução if para que seja tomada uma única decisão cujo resultado será verdadeiro ou falso.

| Operadores lógicos | Significado |
| ------------------ | ----------- |
| !                  | not         |
| &&                 | and         |
| \|\|               | or          |

Onde condicional significa que a linguagem só testará o segundo lado se o primeiro lado for verdadeiro (no caso do and) ou falso (no caso do or).

| Operadores de Comparação | Significado           |
| ------------------------ | --------------------- |
| >                        | maior que             |
| <                        | menor que             |
| >=                       | maior ou igual        |
| <=                       | menor ou igual        |
| ==                       | igual                 |
| !=                       | não igual (diferente) |
| =~                       | checa padrão          |

Alguns outros tipos de ifs utilizados no bash utilizam outros tipos de operadores de Comparação, como veremos abaixo:

| Operadores de Comparação | Significado                |
| ------------------------ | -------------------------- |
| -gt                      | maior que                  |
| -lt                      | menor que                  |
| -ge                      | maior ou igual             |
| -le                      | menor ou igual             |
| -eq                      | equivalente/igual          |
| -ne                      | não igual (diferente)      |
| -d                       | arquivo é diretório        |
| -e                       | arquivo existe             |
| -z                       | arquivo vazio              |
| -f                       | arquivo contém texto       |
| -o                       | usuário é dono do arquivo  |
| -r                       | arquivo pode ser lido      |
| -w                       | arquivo pode ser alterado  |
| -x                       | arquivo pode ser executado |

## Exemplos:

```bash
#! /bin/bash

DINHEIRO=120
VALOR=100

if (( $DINHEIRO >= $VALOR ))
then
    echo "Você acabou de adquirir um fone de ouvido novo"
else
    echo "Você ainda não possui dinheiro para comprar este fone de ouvido"
fi


```
E agora, na  prática da diferença de "-eq" no qual compara inteiros com "==" em que compara as string em si:

```bash
#! /bin/bash

if [ 01 -eq 1 ]
then
    echo "01 equivale a 1"
fi
if [ 01 == 1 ]
then
    echo "01 é igual a 1"
else
    echo "01 não é igual a 1"
fi

```

Utilizando o operador "=~" para validar um email usando Expressões Regulares (Regex).

```bash
#! /bin/bash

EMAIL="bash4noobs@example.com"

if [[ $EMAIL =~ ^[A-Za-z0-9]+@[A-Za-z0-9]+\.[A-Za-z]+$ ]]
then
    echo "O email é válido"
else
    echo "O email não é válido"
fi

```

Note que alguns dos comandos utilizados acima serão vistos posteriormente!

<p align="center">
  <a href="04-Operadores-aritméticos.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="06-Instruções-condicionais.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>
