# 'Semana do Javascript Master'

#### _Evento cujo objetivo é a fluência em Javascript puro._

Ministrado por Roger Melo [![GitHub Badge](https://img.shields.io/badge/GitHub-100000?style=flat-square&logo=GitHub&logoColor=white&link=https://github.com/roger-Melo/)](https://github.com/roger-Melo/)

&nbsp;

### Proposta de 'lista de exercícios'

01 - Gere um novo array com apenas os números ímpares do array abaixo e exiba o novo array no console.

```javascript
const randomNumbers = [10, 30, 15, 25, 50, 40, 5];
```

&nbsp;
Resolução: :heavy_check_mark:

```javascript
const getOddNumbers = (randomNumber) => randomNumber % 2 === 1;
const oddNumbers = randomNumbers.filter(getOddNumbers);
console.log(oddNumbers);
```

&nbsp;
&nbsp;

02 - Exiba no console quantos números abaixo de 501 o array abaixo possui.

```javascript
const crazyNumbers = [937, 5, 395, 402, 501, 333, 502, 781, 3, 691];
```

&nbsp;
Resolução: :heavy_check_mark:

```javascript
const countNumbersLess501 = (accumulator, crazyNumber) => {
  return crazyNumber < 501 ? ++accumulator : accumulator;
};

const numbersLess501 = crazyNumbers.reduce(countNumbersLess501, 0);
console.log(numbersLess501);
```

&nbsp;
&nbsp;

03 - Gere um novo array com cada um dos números abaixo elevados ao quadrado e exiba o novo array no console.

```javascript
const numbers = [5, 7, 3];
```

&nbsp;
Resolução: :heavy_check_mark:

```javascript
const squareNumbers = numbers.map((number) => number ** 2);
console.log(squareNumbers);
```

&nbsp;
&nbsp;

04 - Utilizando o array abaixo, gere um novo array com apenas os filmes lançados antes do ano 2000 e exiba o novo array no console.

```javascript
const tarantinoMovies = [
  { name: "Bastardos inglórios", release: 2009 },
  { name: "Pulp Fiction", release: 1994 },
  { name: "Kill Bill: Volume 2", release: 2004 },
  { name: "Quatro Quartos", release: 1995 },
  { name: "Sin City", release: 2005 },
  { name: "Era uma Vez em... Hollywood", release: 2019 },
  { name: "Django Livre", release: 2012 },
  { name: "Cães de Aluguel", release: 1992 },
  { name: "À Prova de Morte", release: 2007 },
  { name: "Kill Bill: Volume 1", release: 2003 },
];
```

&nbsp;
Resolução: :heavy_check_mark:

```javascript
const moviesReleasedBefore2000 = tarantinoMovies.filter(
  ({ release }) => release < 2000
);
console.log(moviesReleasedBefore2000);
```
