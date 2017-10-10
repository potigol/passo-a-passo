# Primeiros passos

1-	Leia um número e exiba seu sucessor.

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



2- Calculando a média final de um aluno. Dadas as notas dos 4 bimestre; identificando a situação do aluno como: `APROVADO (nota) >=5;  REPROVADO (nota) <5;      MÉDIA(nota)>=5.`

>   :shrimp: Para montar nosso programa, nós precisamos de quatro (4) variáveis que irão receber os valores correspondentes às notas de cada bimestre. 

````python
n1 = leia_real
n2 = leia_real
n3 = leia_real
n4 = leia_real
````

>   :shrimp: Outra possibilidade de montar esse primeiro passo é usando a formula a baixo. Nela, colocamos de uma única vez todos os valores que vamos trabalhar.

````python
n1, n2, n3, n4 = leia_real`
````
>   :shrimp: Usamos `leia_real`, por que os números correspondentes aos valores das notas podem estar no formato de números reais (9,3; 5,7; 8,2;...).

````python
n1+ n2+ n3+n4 / 4 = media`
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
