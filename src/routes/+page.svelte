<script>
  export let title = "BEM-VINDO AO MUNDO DO VÔLEI! 🏐 ";
</script>

<main>
  <h1>{title}</h1>
  <img src="volei.jpg" alt="Imagem" />
  <h1>EXPLORE TUDO SOBRE O VÔLEI OLÍMPICO! 🏐</h1>
  <div class="buttons">
    <a href="/jogadores" class="btn"><h1>Jogadores Famosos</h1></a>
    <a href="/historia" class="btn"><h1>História do Vôlei</h1></a>
    <a href="/loja" class="btn"><h1>Loja</h1></a>
  </div>

</main>

<style>
  main {
    text-align: center;
    margin: 2rem;
  }
  .buttons {
    display: flex;
    justify-content: center;
    gap: 100px;
  }
  .btn {
    display: inline-block;
    padding: 80px 160px;
    background-color: #09af17c2;
    color: white;
    text-decoration: none;
    border-radius: 40px;
  }
</style>
  