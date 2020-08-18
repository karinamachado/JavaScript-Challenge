# JavaScript-Challenge
Control Flow/ Function Exercise.

#### 1)Escreva uma função greetWorld(), a função não deve ter parâmetros e retornar a string 'Hello, World!'.

```
function greetWorld(){
  return 'Hello World!'
}

console.log(greetWorld());
```

  

#### 2)A idade mínima mais comum para votar é 18 anos. Escreva uma função canIVote()que receba um número, representando a idade da pessoa, e retorne o booleano true se ela tiver 18 anos ou mais e o booleano false se não tiver.  
    
```
const canIVote = age => {
    if (age >= 18) {
        return true
    } else {
        return false
    }
}

```

#### 3)Escreva uma função agreeOrDisagree(),que recebe duas strings e retorna 'You agree!'se as duas strings são iguais e 'You disagree!'se as duas strings são diferentes.

```
const agreeOrDisagree = (first, second) => {
    if (first === second) {
        return 'You agree!'
    } else {
        return 'You disagree!'
    }
}

console.log(agreeOrDisagree("yep", "yep"));

/*

// As a function declaration:
function agreeOrDisagree(first, second) {
   if (first === second) {
        return 'You agree!'
    } else {
        return 'You disagree!'
    }
}

*/


// As a ternary: 
const agreeOrDisagree = (first, second) => (first === second) ? 'You agree!' : 'You disagree!'
*/

```


#### 4)Escreva uma função lifePhase()que leva a idade da pessoa,como um número e retorna em que fase da vida ela se encontra.

Aqui estão as classificações:
- 0-3 deve retornar 'baby'
- 4-12 deve retornar 'child'
- 13-19 deve retornar 'teen'
- 20-64 deve retornar 'adult'
- 65-140 deve retornar 'senior citizen'
- Se o número for menor que 0 ou maior que 140, o programa deve retornar 'This is not a valid age'

```
const lifePhase = age => {
    if (age < 0 || age > 140) {
        return 'This is not a valid age'
    } else if (age < 4) {
        return 'baby'
    } else if (age < 13) {
        return 'child'
    } else if (age < 20) {
        return 'teen'
    } else if (age < 65) {
        return 'adult'
    } else {
        return 'senior citizen'
    }
}

```

#### 5)Escreva uma função finalGrade():

- pegue três argumentos do tipo número
- encontre o average desses três números
- retorna a letra da nota (como uma string) a que average corresponde
- return 'Você digitou uma nota inválida.' se qualquer uma das três notas for menor que 0 ou maior que 100

- 0-59 deve retornar: 'F'
- 60-69 deve retornar: 'D'
- 70-79 deve retornar: 'C'
- 80-89 deve retornar: 'B'
- 90-100 deve retornar: 'A'

```

const finalGrade = (midterm, final, homework) => {
    if ((midterm < 0 || midterm > 100) || (final < 0 || final > 100) || (homework < 0 || homework > 100)) {
        return 'You have entered an invalid grade.'
    }
    let average = (midterm + final + homework) / 3
    if (average < 60) {
        return 'F'
    }
    else if (average < 70) {
        return 'D'
    }
    else if (average < 80) {
        return 'C'
    }
    else if (average < 90) {
        return 'B'
    } else {
        return 'A'
    }
}

console.log(finalGrade( 90, 80, 70));


```


#### 6)Escreva uma função reportingForDuty()que tem dois parâmetros de string, ranke lastName, e retorna uma string no seguinte formato: 'rank lastName reporting for duty!'

```
const reportingForDuty = (rank, lastName) => `${rank} ${lastName} reporting for duty!`

console.log(reportingForDuty('Private', 'Fido'));

```
