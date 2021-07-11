# 3.6 Instruções Condicionais

As instruções condicionais são utilizados quando é trazer lógica de maneira mais simples ao nosso código, como foi visto no capítulo anterior.

É importante frizar que, o Bash possui algumas maneiras de utilizar estas instruções e abaixo abordaremos algumas delas:

## if-then-else

Uma instrução if identifica qual instrução executar com base no valor de uma expressão booleana.

É possível utilizar simplesmente uma função if-else sem mais nem menos.

Além disso, o if possui duas formas de se escrever, observaremos melhor ambas nos exemplos abaixo:

### Exemplo 1:

```bash
#! /bin/bash

DINHEIRO=120
VALOR=100

if (( $DINHEIRO > $VALOR ))
then
    echo "Você acabou de adquirir um fone de ouvido novo"
elif (($DINHEIRO == $VALOR))
then
    echo "Você acabou de adquirir um fone novo mas está sem nenhum dinheiro"
else
    echo "Você ainda não possui dinheiro para comprar este fone de ouvido"
fi

```

Alguns Shells não permitem o operador `(())` portanto é necessário usar um outro tipo de if, como veremos no exemplo a seguir.

### Exemplo 2:

```bash
#! /bin/bash

DINHEIRO=120
VALOR=100

if [ $DINHEIRO -ge $VALOR ]
then
    echo "Você acabou de adquirir um fone de ouvido novo"
else
    echo "Você ainda não possui dinheiro para comprar este fone de ouvido"
fi
```

## Switch-Case:

Uma instrução Switch-Case identifica qual instrução executar com base no valor de uma expressão de qualquer tipo.

No geral o Switch-Case é utilizado como alternativa ao if-else, muitas vezes por organização de código quando há muitos casos aninhados.

### Estrutura geral de um switch-case:

- Case valor in: A variável `valor` será responsável por definir qual case será acessado.
- 1): caso a variável valor seja igual a 1, entraremos neste case.
- dois): caso a variável valor seja igual a dois, entraremos neste case.
- \*): caso não haja nenhum case referente é variável valor, este caso será executado.

### Exemplo:

```bash
#! /bin/bash

VARIAVEL=dois

case $VARIAVEL in
    1) echo "um" ;;
    dois) echo "2" ;;
    tres) echo "3" ;;
    quatro) echo "4" ;;
    5) echo "cinco" ;;
    6|SEIS|Seis|seis) echo "6" ;;
    sete) echo "7" ;;
    oito) echo "8" ;;
    nove) echo "9" ;;
    dez) echo "10" ;;
    *) echo "Opcao Invalida!" ;;
esac
```

Para testar melhor este último código, altere o valor da `VARIAVEL` para verificar qual o valor da saída.

<p align="center">
  <a href="05-Operadores-lógicos.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="07-Estruturas-de-repetição.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>