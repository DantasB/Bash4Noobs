# 3.8 Controle de loop

Tal como outras linguagens de programação, os comandos de repetição do bash possuem 2 palavras reservadas para controle de loop, sendo elas: `break`e `continue`.

A necessidade de utilização desses comandos se baseia conforme a necessidade do loop, e estes funcionam quase igual a outras linguagens de programação.

A diferença é que ambas podem receber parâmetros que indicam qual será o loop que será parado (no caso do break) ou que será continuado (no caso do continue), observaremos melhor alguns dos exemplos abaixo:

### Exemplo 1

```bash
#!/bin/bash

A=0

while [ $A -lt 10 ]
do
    echo $A
    if [ $A -eq 5 ]
    then
        break
    elif (($A == 1))
    then
        echo "O Valor obtido é 1"
    fi
    A=`expr $A + 1`
done
```

### Exemplo 2

```bash
#!/bin/bash

NUMS="1 2 3 4 5 6 7"

for NUM in $NUMS
do
    Q=`expr $NUM % 2`
    if [ $Q -eq 0 ]
    then
        echo "Número $NUM é par!!"
        continue
    fi
    echo "Número $NUM é impar"
done
```

### Exemplo 3

```bash
#!/bin/bash

for i in 1 2 3
do
    for j in 0 5
    do
        if (($i==2 && j==0))
        then
            break 2
        else
            echo "$i $j"
        fi
    done
done
```

<p align="center">
  <a href="07-Estruturas-de-repetição.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="../4-Intermediário/01-Variáveis-especiais.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>