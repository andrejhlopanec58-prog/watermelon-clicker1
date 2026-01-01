<div id="game">
  <h1>Собрано арбузов: <span id="score">0</span></h1>
  <img id="watermelon" src="watermelon.png" style="width: 200px; cursor: pointer;">
</div>

<script>
  let score = 0;
  const scoreElement = document.getElementById('score');
  const img = document.getElementById('watermelon');

  img.addEventListener('click', () => {
    score++;
    scoreElement.innerText = score;
    // Добавьте простую анимацию прыжка
    img.style.transform = "scale(0.95)";
    setTimeout(() => img.style.transform = "scale(1)", 50);
  });
</script>
