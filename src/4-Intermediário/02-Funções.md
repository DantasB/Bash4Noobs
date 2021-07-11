# 4.2 Funções

Tal como outras linguagens de programação, bash não fica pra trás e também permite que o usuário escreva suas próprias funções, também permitindo funções recursivas e não recursivas.

Para construi-las é possível observarmos os exemplos abaixo.

### Exemplo 1

```bash
#!/bin/bash

myfunc()
{
  echo "I was called as : $@"
  x=2
}

### Main script starts here

echo "Script was called with $@"
x=1
echo "x is $x"
myfunc 1 2 3
echo "x is $x"
```

### Exemplo 2

```bash
#!/bin/bash

factorial()
{
  if [ "$1" -gt "1" ]; then
    i=`expr $1 - 1`
    j=`factorial $i`
    k=`expr $1 \* $j`
    echo $k
  else
    echo 1
  fi
}


while :
do
  echo "Insira seu número:"
  read x
  factorial $x
done
```

<p align="center">
  <a href="01-Variáveis-especiais.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="03-Arrays.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>