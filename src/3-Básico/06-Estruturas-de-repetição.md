# 3.6 Estruturas de Repetição

Os comandos de repetição são um recurso que permite que um certo trecho do código de um programa dentro deste loop seja repetido um certo número de vezes.
Facilitando gerar códigos mais organizados e lógicas mais complexas.

Em Bash existem quatro comandos de repetição: while, for, until e select.

## While

O `While` é uma estrutura de loop que funciona com um valor condicional instanciado fora do loop.
Esta estrutura irá checar primeiro a condição e, caso a condição seja `true` o código será executado.

### Exemplo

```bash
#!/bin/sh

CONTROL=0

while [ $CONTROL -lt 10 ]
do
   echo $CONTROL
   CONTROL=`expr $CONTROL + 1`
done
```

## For

O `for` é uma estrutura de loop que funciona com um valor condicional instanciado fora do loop.
Esta estrutura irá checar primeiro a condição e, caso a condição seja `true` o código será executado.

### Exemplo

```bash
#! /bin/bash

for variable in 0 1 2 3 4 5 6 7 8 9
do
   echo $variable
done

```

## Until

O `until` é uma estrutura de loop que funciona de forma similar ao do while.
Esta função irá verificar a condição e irá repitir o loop até que esta condição ocorra.

### Exemplo

```bash
#! /bin/bash

A=0

until [ ! $A -lt 10 ]
do
   echo $A
   A=`expr $A + 1`
done
```

## Select

O `select` é uma estrutura de loop que funciona um pouco diferente das outras estruturas.
Esta função em específico irá iterar cada objeto que está na lista, como podemos observar melhor no exemplo abaixo:

### Exemplo

```bash
#! /bin/bash

select DRINK in tea cofee water juice appe all none
do
   echo $DRINK
done
```
