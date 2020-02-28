<script>
  let nome = "Luiz Carlos";
  let idade = 49;
  let titulo = "Professor";
  let descricao = "Um ótimo professor. Dá boas notas.";
  let imagem = "https://avatars0.githubusercontent.com/u/5073025?s=460&v=4";
</script>

<style>
  .card {
    box-shadow: 0 2px 8px rgba(0, 0, 0, 1);
    max-width: 30rem;
    border-radius: 5px;
    margin: 2rem 0;
  }
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 7rem;
  }
  .foto {
    width: 100px;
  }
</style>

<h1>Alô {nome}, minha idade é {idade}.</h1>
<input type="text" bind:value={nome} />
<br />
<input type="text" bind:value={idade} />
<br />
<input type="text" bind:value={imagem} size="100" />
<br />
<input type="text" bind:value={titulo} />
<br />
<textarea bind:value={descricao} />

<div class="card">
  <header>
    <div>
      <img class="foto" src={imagem} alt={nome} />
    </div>
    <div>
      <h1>{nome}</h1>
      <h2>{titulo}</h2>
    </div>
  </header>
  <div>
    <p>{descricao}</p>
  </div>
</div>
