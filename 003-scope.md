## Escopos em JavaScript

O escopo em programação é uma medida da acessibilidade e visibilidade das variáveis, funções e objetos em diferentes partes do código. Existem dois tipos principais de escopo: global e local.

O escopo global abrange variáveis acessíveis em todo o código, independentemente de onde foram declaradas. Por outro lado, o escopo local refere-se a variáveis acessíveis apenas dentro de uma função específica ou bloco de código delimitado por chaves ({ }).

### Tipos de Escopo

#### Escopo Global
O escopo global em JavaScript refere-se à acessibilidade de variáveis fora de qualquer função, o que significa que essas variáveis podem ser acessadas de qualquer lugar no código.

ex.:
```javascript
var globalVar = "Esta é uma variável global";

function minhaFuncao() {
    console.log(globalVar); // A variável globalVar pode ser acessada aqui
}

minhaFuncao(); // Saída: Esta é uma variável global

console.log(globalVar); // Também pode ser acessada aqui fora da função
```

#### Escopo de Bloco
O escopo de bloco é um conceito introduzido no ECMAScript 6 (também conhecido como ES6 ou ES2015) que define o escopo de uma variável para o bloco mais próximo, delimitado por chaves { }. Antes do ES6, o escopo de uma variável em JavaScript era determinado apenas por funções.

```javascript
if (true) {
    let scopedVar = "Esta é uma variável de escopo de bloco";
    console.log(scopedVar); // A variável scopedVar é acessível aqui dentro do bloco if
}

console.log(scopedVar); // Isso resultará em um erro, pois scopedVar está fora do escopo neste ponto
```

### Conclusão

O conceito de escopo é fundamental em JavaScript, determinando a acessibilidade e visibilidade de variáveis, funções e objetos em diferentes partes do código. Compreender a distinção entre escopo global e escopo local é essencial para evitar conflitos de variáveis e para escrever um código mais limpo e organizado.

No escopo global, variáveis são acessíveis de qualquer lugar no código, o que pode ser útil, mas também perigoso se não for gerenciado corretamente, pois pode levar a sobreposição e dificuldades de manutenção. O escopo de bloco, introduzido no ECMAScript 6, proporciona um controle mais preciso sobre a visibilidade das variáveis, restringindo-as ao bloco de código mais próximo delimitado por chaves `{ }`. Isso promove melhores práticas de programação, reduzindo o risco de erros e aumentando a clareza do código.

Em resumo, entender e aplicar corretamente os diferentes tipos de escopo ajuda a criar programas JavaScript mais robustos e menos propensos a erros, facilitando a manutenção e a evolução do código ao longo do tempo.
