# 4.4 Debug

No Bash, também é possível mapear o motivo do seu script falhar utilizando alfumas features de debug, como o parâmetro -x ao executar o script inteiro no modo debug. 

Na tabela abaixo veremos melhor um pouco sobre cada uma dessas flags e o que elas fazem: 

| Flags               | Significado                                                                      |
| ------------------- | -------------------------------------------------------------------------------- |
| -x                  | Executa o script em modo debug                                                   |
| -f                  | Disabilita a geração do nome de arquivos usando caracteres especiais (*, !, etc) |
| -v                  | Imprime o input do shell após receber um input                                   |

Além disso, existe o comando `set`. Este, junto do `-` ou `+` permitem habilitar a flag ou desabilitar respectivamente. Deste modo, dentro do seu código, você consegue ativar e desativar livremente cada uma das flags mostradas acima.

Para entender melhor o funcionamento, podemos observar o código abaixo:

### Exemplo 1

```bash
#!/bin/sh

A=0
set -x

echo "Estou sendo debugado"

while [ $A -lt 10 ]
do
    echo $A
    if [ $A -eq 5 ]
    then
        break
    elif (($A == 1))
        echo "O Valor obtido é 1"
    then
    fi
    A=`expr $A + 1`
done
set +x

echo "Não estou sendo debugado"
```