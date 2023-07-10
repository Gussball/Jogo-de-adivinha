# Jogo de Adivinhação - Número de 0 a 1000
Este é um jogo de adivinhação implementado em JavaScript que roda em um prompt no navegador. O objetivo do jogo é adivinhar um número gerado aleatoriamente, que varia de 0 a 1000. O jogo fornecerá dicas para ajudar o jogador a chegar mais perto da resposta correta.

## Funcionalidades
Geração de um número aleatório entre 0 e 1000.
Recebimento de palpites do jogador através do prompt.
Verificação da resposta do jogador e fornecimento de dicas.
Contagem do número de tentativas do jogador.
Finalização do jogo quando o jogador adivinhar corretamente o número.

## Tecnologias Utilizadas
Linguagem de programação: JavaScript

## Instruções de Uso
Abra o seu navegador web.
Crie um novo documento HTML.
Dentro da tag <script>, cole o código JavaScript fornecido abaixo:
javascript
Copy code
// Gera um número aleatório entre 0 e 1000
const numeroAleatorio = Math.floor(Math.random() * 1001);

let numeroTentativas = 0;
let palpite;

do {
  // Solicita um palpite ao jogador através do prompt
  palpite = parseInt(prompt("Adivinhe o número (entre 0 e 1000):"));

  if (palpite < numeroAleatorio) {
    alert("Tente um número maior!");
  } else if (palpite > numeroAleatorio) {
    alert("Tente um número menor!");
  }

  numeroTentativas++;
} while (palpite !== numeroAleatorio);

// Mostra uma mensagem de acerto e o número de tentativas
alert(`Parabéns! Você acertou o número em ${numeroTentativas} tentativas.`);

Salve o documento HTML.
Abra o documento HTML no seu navegador.
Um prompt será exibido, solicitando que você adivinhe o número.
Insira um número entre 0 e 1000 e clique em OK.
O jogo fornecerá uma dica para ajudá-lo a chegar mais perto da resposta correta.
Continue fazendo palpites até adivinhar corretamente o número.
Quando você acertar, uma mensagem de parabéns será exibida junto com o número de tentativas que você levou para acertar.
Divirta-se jogando e tente adivinhar o número com o menor número de tentativas possível!

![Mentalista](https://user-images.githubusercontent.com/112123706/216470023-015e865e-317f-41ad-992d-b36bd937c675.png)


