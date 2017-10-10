# Primeiros passos

# 1-	Leia um número e exiba seu sucessor.

>   :shrimp: Para montar nosso programa, precisamos colocar uma variável, onde ela simboliza o número que será digitado,  que até então não sabemos qual será.
>   Nesse caso só sabemos que o número é inteiro.

>Veja esse exemplo:

>   :shrimp: Inicialmente precisamos usar uma variável para poder armazenar o número que será digitado pelo usuário do nosso programa.
>   Usaremos a letra `n` (número).

````python
n = leia_inteiro
````

>   :shrimp: Na linguagem de programação POTIGOL usamos `leia_inteiro` para receber números inteiros. Em nosso exemplo, vamos trabalhar com inteiros. 

````python
escreva n + 1
````

>    :shrimp: `Escreva` é o comando de exibição na tela da linguagem de POTIGOL.

>    :shrimp: OBS: Por que fiz `n + 1`? Bem vamos pensar no problema da questão. A questão nós pede para exibir na tela o sucessor do número que será digitado; como não sabemos qual será tal numero digitado, atribuímos uma variável para receber o número, sendo assim, essa variável `n` mais `+` um `1` torna-se seu sucessor; usamos aqui a lógica matemática (qual quer numero mais 1, vira seu sucessor). Exemplo: vamos supor que `n` é 7, então 7 + 1 forma 8, o numero a ser exibido na tela será 8.; Se `n` for 23, então 23 +1 forma 24, o numero a ser exibido na tela será 24.



# 2- Calculando a média final de um aluno. Dadas as notas dos 4 bimestre.
Identificando a situação do aluno como: `APROVADO (nota) >=5; REPROVADO (nota) <5; MÉDIA(nota)>=5.`

>   :shrimp: Para montar nosso programa, nós precisamos de quatro (4) variáveis que irão receber os valores correspondentes às notas de cada bimestre. 

````python
n1 = leia_real
n2 = leia_real
n3 = leia_real
n4 = leia_real
````

>   :shrimp: Outra possibilidade de montar esse primeiro passo é usando a formula a baixo. Nela, colocamos de uma única vez todos os valores que vamos trabalhar.

````python
n1, n2, n3, n4 = leia_real
````
>   :shrimp: Usamos `leia_real`, por que os números correspondentes aos valores das notas podem estar no formato de números reais (9,3; 5,7; 8,2;...).

````python
n1+ n2+ n3+n4 / 4 = media
````
>   :shrimp: Somaremos as quatro (4) notas e dividiremos por quatro (4), para encontrar a média do aluno.

````python
se media >=5 então
````
>   :shrimp: O `“Se”` é usado na linguagem de programação Potigol, para o caso de se ter mais de uma possibilidade de resultado, esse é o primeiro passo para encontrar o resultado esperado. Caso esse resultado não for encontrado aqui, passaremos para o passo seguinte, usando o `”Senão”`.

````python
escreva “Aprovado”
````

>   :shrimp: Se a média do aluno for maior `(>)` ou igual `(=)` a cinco (5) o programa exibirá na tela “Aprovado”. 

````python
senão
````

>   :shrimp: Usamos o `“Senão”` como segunda possibilidade; nesse caso, ele corresponde ao não êxito da primeira possibilidade. 

````python
escreva “Reprovado”
````

>   :shrimp: Se a média do aluno for menor `(<)` a cinco (5), o programa exibirá na tela “Reprovado”.

>   :shrimp: OBS: Para solucionar a questão acima, usamos o seguinte raciocínio, temos quatro (4) números, onde cada um corresponde à nota de um bimestre; notas essas que podem ou não aparecer em formato de números reais, por esse motivo usamos `leia_real`, que na linguagem de Potigol é o comando para trabalhar com números reais. Para encontrar a média final do aluno pegamos os quatro (4) valores correspondentes às notas somamos e dividimos por quatro, isso por que temos quatro bimestres. Caso essa média seja maior que cinco (5), que é a media final para aprovação (uso do `“se”`), o aluno será aprovado, caso não (uso do `“senão”`), reprovado. 


# 3- Calcular a quantidade de dinheiro gasta por um fumante.
Dados: o número de meses que ele fuma; o número de cigarros fumados por dia e o preço de uma carteira.

>   :shrimp: De inicio nós precisamos criar essa pequena tabelinha para usarmos como referencia no desenrolar da questão. Essa é a tabelinha que usaremos inicialmente. 

````html
MF (Numero de meses que fuma)
FD (Cigarros fumados por dia)
V (Valor da carteira)
````

>   :shrimp: Nosso programa ira receber três valores a serem digitados pelo usuário. 

````python
MF = leia_inteiro
FD = leia_inteiro
V = leia_real
````

>   :shrimp: Usamos o comando `leia_real`, pois o valor a ser digitado poderá ser digitado no formato de números reais (2,74; 3,50; 4,35...).

>   :shrimp: Segundo momento: Criaremos essa nova tabela para atribuir siglas as novas ações que teremos que desenvolver. 

````html
NCF (Numero de carteiras fumadas por mês)
QJF (Quantidade de carteira já fumada)
VG (Valor gasto)
````
>   :shrimp: Após o usuário digitar os valores necessários, vamos gerar novos valores para encontrar o valor gasto por ele com o uso do cigarro.
As variáveis `NCF`, `QJF` e `VG `precedem a operação matemática por estarem recebendo os valores gerados pela operação. Exemplo: NCF recebera o valor do resultado de FD multiplicado por trinta (30) e dividido por vinte (20). Sendo assim, `NFC` será para nosso programa um valor, que é o valor resultante dessa operação. 

>   :shrimp: Vamos encontrar o numero de cigarros fumados; multiplicaremos o numero de cigarros fumados por dia por trinta (quantidade de dias que um mês possui) acharemos um valor total de cigarros fumados num mês, esse valor dividiremos por vinte (quantidade de cigarros que uma carteira possui) assim teremos a quantidade de carteiras fumadas em um mês. 

````python
NCF = (FD * 30) / 20
````

>   :shrimp: Para achar a quantidade de careira já fumada `(QJF)`, usaremos o valor de `NCF` (quantidade de carteira fumada em um mês) vezes o valor nos dado pelo usuário ao `MF` (numero de meses que fuma).

````python
QJF = NCF * MF 
````

>   :shrimp: Agora que temos todos os valores necessários para dá à resposta de quanto o usuário gasta/gastou até então fumando, vamos multiplicar o `QJF` (quantidade já fumada) vezes `V` (valor de cada carteira) para encontrar `VG` (valor total gasto).

````python
VG = QJF * V 
````

>   :shrimp: Para exibir a nosso usuário o resultado, usaremos o comando `“escreva”` para o nosso programa exibir na tela. 

````python
escreva VG
````

>   :shrimp: OBS: Vamos entender a lógica usada na solução desse problema: Nós precisávamos que nosso usuário nos desse os valores iniciais para encontrarmos a resposta. Solicitamos valores necessários como: valor de uma carteira de cigarros; há quantos meses ele fumava e quantos cigarros ele fuma por dia. Tendo esses valores iniciais, construímos novos valores dentro de nosso programa, exemplo: numero de carteiras fumadas num mês, achamos esse valor multiplicando o numero de cigarros fumados por dia vezes 30, assim temos um número total de cigarros; sabendo que uma carteira possui 20 cigarros, dividimos o valor encontrado por vinte, assim achamos a quantidade de carteiras por mês; depois foi só calcular pela quantidade de meses que ele fuma achando a quantidade de carteiras fumada em todo o tempo e depois foi só multiplicar pelo valor de cada carteira.

