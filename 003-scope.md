## Escopo em JavaScript

Escopo refere-se à acessibilidade e visibilidade de variáveis, funções e objetos em diferentes partes do código. Existem dois tipos principais de escopo: global e local. Escopo global refere-se a variáveis acessíveis em todo o código, enquanto escopo local refere-se a variáveis acessíveis apenas dentro de uma função específica.

## Tipos de Escopo

### **1. Escopo Global:** O escopo global em JavaScript refere-se à acessibilidade de variáveis fora de qualquer função, o que significa que essas variáveis podem ser acessadas de qualquer lugar no código.

ex.:
```javascript
var globalVar = "Esta é uma variável global";

function minhaFuncao() {
    console.log(globalVar); // A variável globalVar pode ser acessada aqui
}

minhaFuncao(); // Saída: Esta é uma variável global

console.log(globalVar); // Também pode ser acessada aqui fora da função
```

* **2. Escopo de Bloco:** O escopo de bloco é um conceito introduzido no ECMAScript 6 (também conhecido como ES6 ou ES2015) que define o escopo de uma variável para o bloco mais próximo, delimitado por chaves { }. Antes do ES6, o escopo de uma variável em JavaScript era determinado apenas por funções.

```javascript
if (true) {
    let scopedVar = "Esta é uma variável de escopo de bloco";
    console.log(scopedVar); // A variável scopedVar é acessível aqui dentro do bloco if
}

console.log(scopedVar); // Isso resultará em um erro, pois scopedVar está fora do escopo neste ponto
```
