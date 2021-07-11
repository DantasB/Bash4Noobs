# 4.3 Arrays

Bash também permite criar arays tal como outras linguagens e, possui o índice inicial definido como 0.

Para esta estrutura de dados, é possível criar utilizando de duas formas, declare ou igual, como veremos melhor nos exemplos abaixo:

### Exemplo 1

```bash
#!/bin/bash

MEU_ARRAY=('A' 'B' 'C' 'D' 'E')

echo ${MEU_ARRAY[2]}
```

Também é possível utilizar algumas das variáveis especiais explicada como argumentos do array, podendo então acessar facilmente todos os elementos do array ou limitar quais elementos você quer acessar.

### Exemplo 2

```bash
#!/bin/bash

declare -a MEU_ARRAY=('A' 'B' 'C' 'D' 'E')

echo ${MEU_ARRAY[@]} #Imprime todos os valores do array
```

Além disso, os arrays também permitem sobrescrever seus valores, podendo ser feito da seguinte forma:

### Exemplo 3

```bash
#!/bin/bash

declare -a MEU_ARRAY=('A' 'B' 'C' 'D' 'E')

MEU_ARRAY[2]='K' # Substitui o C pelo K

MEU_ARRAY[5]='F' # Adiciona um novo elemento ao final do array com o valor F

echo ${MEU_ARRAY[@]}
```

Além disso, possuem uma série de comandos para arrays, como o comando `unset` que permite apagar elementos do array com base no id fornecido e o comando `#` que permite obter o número de elementos do array de forma simples\*, como podemos ver abaixo:

\*OBS: O comando `#` também permite obter o número de caracteres em uma string.

### Exemplo 4

```bash
#!/bin/bash

declare -a MEU_ARRAY=('A' 'B' 'C' 'D' 'E')

echo ${#MEU_ARRAY[@]} # A saída será 5 pois temos 5 elementos em todo o array

unset MEU_ARRAY[2] # Remove o elemento de índice 2 do array

echo ${#MEU_ARRAY[@]} # A saída será 4 pois removemos o elemento de indice 2 do array.


echo ${MEU_ARRAY[@]}
```

Finalmente, mas não tão importante, bash permite slicing (algo encontrado em python), fazendo com que seja possível pegar fatias do array.

### Exemplo 5

```bash
#!/bin/bash

declare -a MEU_ARRAY=('A' 'B' 'D' 'E')

echo ${MEU_ARRAY[@]:1:2} # A saída B D, pois estamos pegando dentro do array o elemento 1 até o elemento 2 do array

echo ${MEU_ARRAY[@]:2} # A saída será D E, pois estamos pegando do elemento de id 2 até o último elemento do array

echo ${MEU_ARRAY[@]:-1} # A saída será E, pois estamos pegando o último elemento do array (similar ao python)

```

<p align="center">
  <a href="02-Funções.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605852304048148/anterior.png" height=35>
  </a>
  <a href="04-Debug.md">
    <img src="https://cdn.discordapp.com/attachments/539836343094870016/863605863049461780/proximo.png" height=35>
  </a>
</p>