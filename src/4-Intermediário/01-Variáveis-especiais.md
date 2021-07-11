# 4.1 Variáveis Especiais

O Bash possui algumas variáveis especiais que permitem você acessar informações do próprio sistema operacional dentro do código, além de acessar as variáveis de input de forma única.

Nesta tabela, você poderá encontrar e descobrir como utilizar algumas dessas variáveis no exemplo mais abaixo.

| Variáveis Especiais | Significado                                                                                      |
| ------------------- | ------------------------------------------------------------------------------------------------ |
| $1 ... $n           | Acessa os parâmetros de input do programa. $0 acessa o primeiro, $1 o segundo e assim em diante. |
| $IFS                | Altera o separador do texto. Em vez de espaço pode ser o que você definir.                       |
| $@                  | Imprime todos os parâmetros passados para a função.                                              |
| $\*                 | Tem o mesmo comportamento do $@ porém troca os espaços em branco por aspas duplas.               |
| $#                  | Número de parâmetros que o script recebeu.                                                       |
| $0                  | Nome do programa executado.                                                                      |
| $!                  | Retorna o PID do último programa executado.                                                      |
| $$                  | Retorna o PID do processo sob o qual o script está sendo executado.                              |
| $?                  | Output do ultimo programa executado.                                                             |

<p align="center">
  <a href="../3-Básico/08-Controle-de-loop.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="02-Funções.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>