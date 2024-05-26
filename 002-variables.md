## O que são variáveis?

Variáveis são espaços na memória do computador designados para armazenar informações com base no contexto em que estão inseridas. Em linguagens de programação, como JavaScript, as variáveis são como caixas onde podemos guardar diferentes tipos de dados, como números, textos e objetos. Assim como na vida real, podemos atribuir valores a essas caixas e depois acessá-los conforme necessário.

## Como declarar uma variável em JavaScript?

Em JavaScript, existem três palavras-chave para declarar variáveis: `var`, `let`, e `const`. Cada uma delas tem suas próprias características de escopo e comportamento, o que influencia como a variável pode ser usada no código.

## Tipos de variáveis

- **VAR**: uma variável global acessível em toda a aplicação. Porém, seu uso é desencorajado devido ao seu escopo global, que pode levar a problemas devido a possíveis sobreposições de variáveis.
- **LET**: uma variável de escopo de bloco, acessível apenas dentro do bloco onde é definida. Recomendada para variáveis que terão seus valores alterados ao longo do código.
- **CONST**: uma variável de valor constante e escopo de bloco, ideal para manter valores imutáveis na aplicação. Uma vez atribuído, o valor de uma constante não pode ser alterado.

## Regras para nomear uma variável

Ao nomear variáveis em JavaScript, é importante seguir algumas regras para garantir consistência e legibilidade no código:

- Devem começar com uma letra de a-z, \_, ou $;
- Podem conter letras de a-z (maiúsculas e minúsculas), números de 0-9;
- As variáveis são sensíveis a maiúsculas e minúsculas.

## Como declarar uma variável?

A declaração de uma variável em JavaScript segue uma sintaxe simples. Indicamos o tipo de variável, seguido pelo nome e, opcionalmente, um valor inicial.

```javascript
// Exemplo de declaração de variáveis em JavaScript
var x = 10; // variável var
let y = 20; // variável let
const z = 30; // variável const
```
