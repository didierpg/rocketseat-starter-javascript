# Exercícios: Módulo 01
## 1º exercício
### Crie uma função que dado o objeto a seguir:
```javascript 
var endereco = {
 rua: "Rua dos pinheiros",
 numero: 1293,
 bairro: "Centro",
 cidade: "São Paulo",
 uf: "SP"
};
```
### Retorne o seguinte conteúdo:
```
O usuário mora em São Paulo / SP, no bairro Centro, na rua "Rua dos Pinheiros" com nº 1293.
```
## 2º exercício
### Crie uma função que dado um intervalo (entre x e y) exiba todos número pares:
```javascript 
function pares(x, y) {
 // código aqui
}
pares(32, 321);
```
## 3º exercício
### Escreva uma função que verifique se o vetor de habilidades passado possui a habilidade "Javascript" e retorna um booleano true/false caso exista ou não.
```javascript 
function temHabilidade(skills) {
 // código aqui
}
var skills = ["Javascript", "ReactJS", "React Native"];
temHabilidade(skills); // true ou false
```
*Dica: para verificar se um vetor contém um valor, utilize o método [indexOf](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf).*
## 4º exercício
### Escreva uma função que dado um total de anos de estudo retorna o quão experiente o usuário é:
```javascript
function experiencia(anos) {
 // código aqui
}
var anosEstudo = 7;
experiencia(anosEstudo);
// De 0-1 ano: Iniciante
// De 1-3 anos: Intermediário
// De 3-6 anos: Avançado
// De 7 acima: Jedi Master
```
## 5º exercício
### Dado o seguinte vetor de objetos:
```javascript
var usuarios = [
 {
 nome: "Diego",
 habilidades: ["Javascript", "ReactJS", "Redux"]
 },
 {
 nome: "Gabriel",
 habilidades: ["VueJS", "Ruby on Rails", "Elixir"]
 }
];
```

### Escreva uma função que produza o seguinte resultado:

```
O Diego possui as habilidades: Javascript, ReactJS, Redux
O Gabriel possui as habilidades: VueJS, Ruby on Rails, Elixir
```
*Dica: Para percorrer um vetor você deve utilizar a sintaxe [for...of](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/for...of) e para unir valores de um array com um separador utilize o [join](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/join).*

# Exercícios: Módulo 02
## 1º exercício
### Crie um botão que ao ser clicado cria um novo elemento em tela com a forma de um quadrado vermelho com 100px de altura e largura. Sempre que o botão for clicado um novo quadrado deve aparecer na tela.
## 2º exercício
### Utilizando o resultado do primeiro desafio, toda vez que o usuário passar o mouse por cima de algum quadrado troque sua cor para uma cor aleatória gerada pela função abaixo:
```javascript
function getRandomColor() {
 var letters = "0123456789ABCDEF";
 var color = "#";
 for (var i = 0; i < 6; i++) {
 color += letters[Math.floor(Math.random() * 16)];
 }
 return color;
}
var newColor = getRandomColor(); // #E943F0
```
## 3º exercício
### A partir do seguinte vetor:
```javascript
var nomes = ["Diego", "Gabriel", "Lucas"];
```
### Preencha uma lista (`<ul>`) no HTML com os itens da seguinte forma:
- Diego
- Gabriel
- Lucas
## 4º exercício
### Seguindo o resultado do exercício anterior adicione um input em tela e um botão como a seguir:
```javascript
<input type="text" name="nome">
<button onClick="adicionar()">Adicionar</button>
```
### Ao clicar no botão, a função `adicionar()` deve ser disparada adicionando um novo item a lista de nomes baseado no nome preenchido no input e renderizando o novo item em tela juntos aos demais itens anteriores. Além disso, o conteúdo do input deve ser apagado após o clique.