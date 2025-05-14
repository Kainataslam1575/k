<canvas id="wheel" width="400" height="400"></canvas>
<script>
  const canvas = document.getElementById('wheel');
  const ctx = canvas.getContext('2d');

  for (let i = 0; i < 360; i += 1) {
    ctx.beginPath();
    ctx.moveTo(200, 200);
    ctx.arc(200, 200, 150, (i-1)*Math.PI/180, i*Math.PI/180);
    ctx.fillStyle = `hsl(${i}, 100%, 50%)`;
    ctx.fill();
  }
</script>
