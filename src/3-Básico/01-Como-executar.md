# 3.1 Como executar

Após definir seu ambiente e entender a história por trás da linguagem bash, neste módulo entraremos mais a fundo na linguagem e entender melhor como ela funciona.

Nos próximos capítulos, você encontrará alguns códigos e será interessante que você tente executa-los em sua máquina, buscando modificar e entender o que foi ensinado no módulo em questão. 

Contudo, é importante que você saiba como executar esses códigos, para que você consiga rodar localmente, como veremos melhor abaixo.


Nos sistemas operacionais UNIX, é necessário que alguns arquivos possuam as permissões de execução para conseguir rodar, caso contrário um erro aparecerá dizendo que este arquivo não possui as permissões necessárias.

Abaixo teremos um tutorial de como executar esses códigos que veremos nos próximos módulos:


```bash

# Após você copiar o código que você pretende executar, crie um arquivo .sh e coloque este conteúdo.
$ nano nome_do_arquivo.sh

# Depois colar todo o código e salvar este arquivo usando o comando CTRL + O, dê a permissão de escrita
$ chmod +x nome_do_arquivo.sh

# Por ultimo você poderá executar o arquivo utilizando ./
$ ./nome_do_arquivo.sh
```

<p align="center">
  <a href="../2-Ambiente/04-Online.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="02-Declaração-de-variáveis.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>