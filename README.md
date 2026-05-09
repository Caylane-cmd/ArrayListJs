# ArrayListJs
Tutorial sobre manipulação de listas em JavaScript utilizando map(), filter() e reduce().

Para esse tutorial irei usar uma problematica parar explicar como fazer a manipulação em uma lista usando os metodos map(), filter() e reduce().

Ex: Uma loja que tem vários produtos precisa filtrar os produtos, listar apenas os nomes e calcular o valor total dos produltos. 

ok, agora que já sabemos do problema vamos iniciar, iremos começar fazendo a variavel "produto" que irá listar o nome e o preço dos produtos.

```js
const produtos = [
  { nome: "Mouse", preco: 50 },
  { nome: "Teclado", preco: 120 },
  { nome: "Monitor", preco: 900 },
  { nome: "Notebook", preco: 3500 }
];
```
## filter
```js
const produtosCaros = produtos.filter(p => p.preco > 100);
console.log(produtosCaros);

Resultado
[
  { nome: "Teclado", preco: 120 },
  { nome: "Monitor", preco: 900 },
  { nome: "Notebook", preco: 3500 }
]
```
O filter() como o nome já sujere ele serve para filtrar elementod de um array. Nesse trecho pegamos o array produtos, e chamamos o metodo filter()ele vai percorrer o array verificando cada número e será retornado um novo array com os elementos que foi estipulado na condição, preços maiores que 100 .

---

## map

```js
const nomes = produtos.map(p => p.nome);
console.log(nomes);

Resultado
["Mouse", "Teclado", "Monitor", "Notebook"]
```
O metodo map() ele transforma os elementos da maneira que queremos.Nesse trexo de código ele vai pegar os elementos (apenas os nomes) do array original e criar um novo array só com nomes dos produtos.

---

## reduce

```js
const total = produtos.reduce((acc, p) => acc + p.preco, 0);
console.log(total);

Resultado
4570
```
O reduce() ele é útio quando queremos que todos os valores da lista pra um só. Nesse trecho de código ele vai pegar todos os preço e somar um a um nos dando apenas o valor total.

