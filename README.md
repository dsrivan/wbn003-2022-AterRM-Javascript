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
