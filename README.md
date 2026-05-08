# ArrayListJs
Tutorial sobre manipulação de listas em JavaScript utilizando map(), filter() e reduce().

Para esse tutorial irei usar uma problematica parar explicar como fazer a manipulação em uma lista usando map(), filter() e reduce().

Ex: Uma loja que tem vários produtos precisa filtrar os produtos, listar apenas os nomes e calcular o valor total dos produltos. 

ok, agora que já sabendo do problema vamos iniciar, iremos começar fazendo a variavel "produto" que irá listar o nome e o preço dos produtos.

```js
const produtos = [
  { nome: "Mouse", preco: 50 },
  { nome: "Teclado", preco: 120 },
  { nome: "Monitor", preco: 900 },
  { nome: "Notebook", preco: 3500 }
];
```
## filter
O filter() ele vai percorre e filtrar de maneira mais limpa funcionarvai receber uma função que vai ser executada pra cada item da lista.O filter()vai chamar o array
