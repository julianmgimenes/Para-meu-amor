❤<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cartinha de Páscoa para o Meu Amor</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background-color: #ffe6f0;
      overflow: hidden;
      font-family: 'Comic Sans MS', cursive, sans-serif;
    }

    /* Elementos flutuantes */
    .floating-item {
      position: absolute;
      animation: float 10s infinite ease-in;
      opacity: 0.8;
    }

    .heart {
      width: 20px;
      height: 20px;
      background: red;
      transform: rotate(45deg);
    }
    .heart::before, .heart::after {
      content: "";
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      border-radius: 50%;
    }
    .heart::before {
      top: -10px;
      left: 0;
    }
    .heart::after {
      top: 0;
      left: -10px;
    }

    .chocolate {
      width: 20px;
      height: 30px;
      background: #6b3e26;
      border-radius: 4px;
      box-shadow: inset 0 0 3px #3e2415;
      position: relative;
    }
    .chocolate::before {
      content: "";
      position: absolute;
      width: 100%;
      height: 8px;
      background: #8b5a2b;
      top: 0;
      border-top-left-radius: 4px;
      border-top-right-radius: 4px;
    }

    .coelhinho {
      width: 20px;
      height: 30px;
      background: #fff;
      border-radius: 10px;
      position: relative;
      box-shadow: inset 0 0 2px #aaa;
    }
    .coelhinho::before, .coelhinho::after {
      content: "";
      position: absolute;
      width: 6px;
      height: 16px;
      background: #fff;
      border-radius: 50% 50% 0 0;
      top: -14px;
      box-shadow: inset 0 0 1px #aaa;
    }
    .coelhinho::before {
      left: 2px;
    }
    .coelhinho::after {
      right: 2px;
    }

    @keyframes float {
      0% {
        transform: translateY(100vh) rotate(0deg);
      }
      100% {
        transform: translateY(-10vh) rotate(360deg);
      }
    }

    /* Moldura de Páscoa nas fotos quadradas */
    .foto-quadrada {
      position: fixed;
      top: 50%;
      width: 160px;
      height: 160px;
      transform: translateY(-50%);
      background-size: cover;
      background-position: center;
      border: 6px solid #ff99bb;
      border-radius: 20px;
      box-shadow: 0 0 20px rgba(255, 0, 85, 0.3);
      z-index: 0;
      overflow: visible;
    }

    /* Elementos decorativos nas quinas */
    .foto-quadrada::before,
    .foto-quadrada::after {
      content: '❤️';
      position: absolute;
      font-size: 30px;
    }
    .foto-quadrada::before {
      top: -20px;
      left: -20px;
    }
    .foto-quadrada::after {
      bottom: -20px;
      right: -20px;
    }

    .foto-quadrada .coelho {
      position: absolute;
      top: -20px;
      right: -20px;
      font-size: 30px;
    }

    .foto-quadrada .ovo {
      position: absolute;
      bottom: -20px;
      left: -20px;
      font-size: 30px;
    }

    /* Cartinha */
    .carta {
      background: white;
      max-width: 500px;
      margin: 50px auto;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 0 20px rgba(255, 0, 85, 0.3);
      text-align: center;
      position: relative;
      z-index: 1;
    }

    h1 {
      color: #ff3366;
      font-size: 2.5em;
      margin-bottom: 20px;
    }

    p {
      color: #333;
      font-size: 1.2em;
      line-height: 1.6;
    }

    .emoji-heart {
      color: red;
      font-size: 1.5em;
    }

    /* Chocolates animados subindo */
    .chocolate-float {
      position: fixed;
      bottom: -50px;
      font-size: 30px;
      animation: subir 5s linear infinite;
      z-index: 10;
      pointer-events: none;
    }

    @keyframes subir {
      0% {
        transform: translateY(0) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(-110vh) rotate(360deg);
        opacity: 0;
      }
    }

    /* Responsividade */
    @media (max-width: 768px) {
      .foto-quadrada {
        width: 120px;
        height: 120px;
      }

      .foto-quadrada::before,
      .foto-quadrada::after,
      .foto-quadrada .coelho,
      .foto-quadrada .ovo {
        font-size: 24px;
      }

      .carta {
        padding: 20px;
        max-width: 400px;
      }

      h1 {
        font-size: 2em;
      }

      p {
        font-size: 1em;
      }
    }
  </style>
</head>
<body>

  <!-- Corações -->
  <div class="floating-item heart" style="left: 10%; animation-delay: 0s;"></div>
  <div class="floating-item heart" style="left: 30%; animation-delay: 2s;"></div>
  <div class="floating-item heart" style="left: 50%; animation-delay: 4s;"></div>
  <div class="floating-item heart" style="left: 70%; animation-delay: 1s;"></div>
  <div class="floating-item heart" style="left: 90%; animation-delay: 3s;"></div>

  <!-- Chocolates flutuantes -->
  <div class="floating-item chocolate" style="left: 20%; animation-delay: 1.5s;"></div>
  <div class="floating-item chocolate" style="left: 60%; animation-delay: 3.5s;"></div>

  <!-- Coelhinhos -->
  <div class="floating-item coelhinho" style="left: 40%; animation-delay: 2.5s;"></div>
  <div class="floating-item coelhinho" style="left: 80%; animation-delay: 0.5s;"></div>

  <!-- Fotos quadradas com moldura temática de Páscoa -->
  <div class="foto-quadrada foto-esquerda" style="left: 10%; background-image: url('formatura.jpg');">
    <span class="coelho">🐰</span>
    <span class="ovo">🥚</span>
  </div>
  <div class="foto-quadrada foto-direita" style="right: 10%; background-image: url('parque.jpg');">
    <span class="coelho">🐰</span>
    <span class="ovo">🥚</span>
  </div>

  <!-- Cartinha -->
  <div class="carta">
    <h1>Feliz Páscoa, meu amor! 🐰🍫</h1>
    <p>
      Preparei essa cestinha de chocolate com todo o carinho, pensando no quanto você é especial pra mim.  
      Que essa Páscoa renove nossos sentimentos, nossa alegria e encha nosso coração de amor e doçura, assim como esses chocolatinhos.  
      Te amo demais! <span class="emoji-heart">❤️❤️❤️</span>
    </p>
  </div>

  <script>
    function criarChocolateFlutuante() {
      const chocolate = document.createElement('div');
      chocolate.classList.add('chocolate-float');
      chocolate.textContent = '🍫';
      chocolate.style.left = Math.random() * 100 + 'vw';
      chocolate.style.animationDuration = (3 + Math.random() * 3) + 's';
      document.body.appendChild(chocolate);

      setTimeout(() => {
        chocolate.remove();
      }, 6000);
    }

    setInterval(criarChocolateFlutuante, 300);
  </script>

</body>
</html>
