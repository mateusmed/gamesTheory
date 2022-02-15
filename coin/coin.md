

Demonstrar programaticamente a mecânica de um jogo de moedas
onde NÃO é percebido intuitivavemente o sistema de conjutos dada a forma de demostração

```
| x | k | k | x |
| k | y | y | k |
| k | y | y | k |
| x | k | k | x |
```

Onde as bordas são uniões dos conjuntos, levando assim a uma estranhesa em aritméticas simples. 
A abstração aplicada, é o conceito de familias, onde temos 4 familias, caracterizadas
pelas linhas e colunas onde existe o X

```
Y = valores para atribuir
X = 'conjunto' de valores de duas famílias
K = valores únicos de uma determinada familia
```

Suponhamos a operação:


```
| 3 | 2 | 2 | 3 |
| 2 | 4 | 4 | 2 |
| 2 | 4 | 4 | 2 |
| 3 | 2 | 2 | 3 | 
```

```
[2][2] = -1
[1][2] = +1
[1][1] = -1
[2][1] = +1
```

logo:

```
familia        C           D
familia A    | 2 | 3 | 2 | 3 |
             | 3 | 3 | 4 | 2 |
             | 2 | 4 | 4 | 2 |
familia B    | 3 | 2 | 2 | 3 | 
```

Por tanto, mesmo atribuindo um novo valor a familia 'A'
e a familia 'A' emprestando um valor para a familia 'C'
ambas permanecem com 10