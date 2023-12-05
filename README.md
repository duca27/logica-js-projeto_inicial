# logica-js-projeto_inicial

Jogo de adivinhação, onde o usuário precisa adivinhar o "número secreto"

| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | **logica-js-projeto_inicial**
| :label: Tecnologias | javascript
| :rocket: URL         | [https://url-deploy.com.br](http://127.0.0.1:5500/index.html)
| :fire: Desafio     | Descubra o número secreto
alert('Saudações terráqueos');
let numeroMáximo = 9000
let numeroSecreto = parseInt (Math.random() * numeroMáximo + 1);
console.log(numeroSecreto);
let chute;
let tentativas = 1;
while (chute != numeroSecreto) {
    chute = prompt(`Escolha um número entre 1 e ${numeroMáximo}`);
    if (chute == numeroSecreto) {
        break;
    } else { 
        if (chute > numeroSecreto) {
            alert(`O número secreto é menor que ${chute}.`);
        } else {
            alert(`O número secreto é maior que ${chute}.`);
        }
        tentativas++;
    } 
}
let palavraTentativa = tentativas > 1 ? 'tentativas' : 'tentativa';
alert(`Isso aí! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} ${palavraTentativa}`);

<!-- Inserir imagem com a #vitrinedev ao final do link -->
![jogo1](https://github.com/duca27/Meus-Projetos/assets/152569671/d6f9d0a4-52f3-4e19-950e-127a572762f4)

