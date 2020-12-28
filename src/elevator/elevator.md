
Demostrar aritmeticas simples usando o tipo de dado Infinity do nodejs

```
const maxNumber = Math.pow(10, 1000); // max positive number

if (maxNumber === Infinity) {
  console.log('Let\'s call it Infinity!');
  // expected output: "Let's call it Infinity!"
}

console.log(1 / maxNumber);
// expected output: 0

console.log(Infinity          ); /* Infinity */
console.log(Infinity + 1      ); /* Infinity */
console.log(Math.pow(10, 1000)); /* Infinity */
console.log(Math.log(0)       ); /* -Infinity */
console.log(1 / Infinity      ); /* 0 */
console.log(1 / 0             ); /* Infinity */
```
---

Hilbert's Paradoxo do hotel infinito.

Para a comparação de conjuntos infinitos, associamos um item do conjunto A com um item do conjunto B 
dessa forma quando um dos conjuntos acabar, logo inferimos que o outro é o maior.


Ao comparar o conjunto infinito dos numeros naturais com os numeros pares, por exemplo:

```
1, 2, 3, 4, 5, 6, 7, 8, 9 ...
2, 4, 6, 8, 10, 12, 14, 15, 16 ...
```

Dada a regra anterior, somos tendenciosos a acreditar que o conjunto dos naturais é maior, 
pois possui todos os numeros incluidos no conjunto dos numeros pares
porém se relacionarmos todos os numeros tendendo ao infinito, nenhum conjunto se caracteriza
maior que o outro.

---

Suponhamos um hotel com um numero de quartos infinito.
- todos esses quartos estão ocupados

Mesmo com todos os quartos ocupados é possível acomodar mais um hóspede.
- Como isso seria possível?


Mais uma vez o problema demostra como o tratamento com números infinitos é totalmente contra intuitivo.

Se pedirmos para o hóspede do quarto número 1 ir para o número 2 e o do quarto número 2 ir para o numero 3
e assim sucessivamente, teremos um quarto disponível

```
  1-> 2-> 3-> 4
|   |   |   |   | ...

      1   2   3   4
| x |   |   |   | ...
```

O mesmo acontece, quando precisamos acomodar um número infinito de novos hóspedes.
O movimento dos quartos seria:

```
N -> 2N
```

Por exemplo, hóspede do quarto 1:

```
(1 = 2.1) = 2
(2 = 2.2) = 4
(3 = 2.3) = 6
...
```

Dessa forma, todos os quartos impares estarão vagos.

