# 3.4 Operadores lógicos e de Comparação

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

Alguns outros tipos de ifs utilizados no bash utilizam outros tipos de operadores de Comparação, como veremos abaixo:

| Operadores de Comparação | Significado           |
| ------------------------ | --------------------- |
| -gt                      | maior que             |
| -lt                      | menor que             |
| -ge                      | maior ou igual        |
| -le                      | menor ou igual        |
| -eq                      | igual                 |
| -ne                      | não igual (diferente) |

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

Note que alguns dos comandos utilizados acima serão vistos posteriormente!
