# 3.2 Declaração de Variáveis

Assim como toda a linguagem de programação possuem variáveis, o Bash não é a exceção. Nesse tópico iremos introduzir a ideia e mais para frente aprofundaremos mais alguns outros tipos de variáveis.

Antes de utilizar uma variável, é necessário, OBRIGATORIAMENTE, declara-la e especificar seu nome.

O Bash, tal como outras linguagens, possui algumas regras de boa nomenclatura de variável. Abordaremos algumas à seguir:

- Um nome de variável DEVE ser feito em UPPER CASE e é considerado boa prática.

- Não use espaços depois da inicialização de uma variável e seu valor.

- Não utilize palavras reservadas como nome de variável (if, else, for, while, int, float, etc.)

- Não use nome de variáveis com espaço.

Além disso, é importante frizar que o nome de variável, tal como outras linguagens de programação é case-sensitive, ou seja, a variável valor é diferente da variável Valor.

```bash
#! /bin/bash

NAME="HE4RT"

echo $NAME
```

Para verificar qual será a saida deste código, execute em seu terminal ou em um dos compiladores sugeridos!

É importante ressaltar que, SEMPRE que formos acessar uma variável, é necessário utilizar o `$` antes da variável.

Veremos mais a frente como funciona o `echo`.

<p align="center">
  <a href="01-Como-executar.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="03-Entrada-e-saída.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>