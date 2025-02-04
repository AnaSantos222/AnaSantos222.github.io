<script>
    let jogadores = [
      { 
        name: "Bernardinho", 
        description: "Considerado um dos maiores técnicos da história do vôlei, Bernardinho foi campeão olímpico como jogador e técnico.", 
        image: "benardinho.jpg",
        link: "https://pt.wikipedia.org/wiki/Bernardinho" 
      },
      { 
        name: "Giba", 
        description: "Ícone do vôlei mundial, Giba conquistou três medalhas olímpicas, sendo duas de ouro.", 
        image: "giba.jpg",
        link: "https://www.esportelandia.com.br/volei/giba-volei/" 
      },
      { 
        name: "Ricardinho", 
        description: "Famoso levantador da seleção brasileira, Ricardinho foi uma peça chave nas conquistas olímpicas.", 
        image: "ricardinho.jpg",
        link: "https://pt.wikipedia.org/wiki/Ricardo_Garcia" 
      },
      { 
        name: "Wallace", 
        description: "O oposto Wallace foi um dos maiores nomes da equipe brasileira nas Olimpíadas de 2016, conquistando ouro no Rio.", 
        image: "wallace.jpg",
        link: "https://www.cob.org.br/time-brasil/medalhistas-olimpicos/wallace-leandro-de-souza" 
      },
      { 
        name: "Darlan", 
        description: "Jovem promessa do vôlei brasileiro, Darlan vem ganhando destaque nas Olimpíadas recentes e promete brilhar mais.", 
        image: "darlan.jpg",
        link: "https://ge.globo.com/olimpiadas/guia/2024/07/27/c-darlan-souza-altura-idade-peso-time-posicao-e-historia.ghtml" 
      },
    ];
  </script>
  
  <main>
    <h1>Jogadores de Vôlei Brasileiro nas Olimpíadas</h1>
    <ul>
      {#each jogadores as jogador}
        <li>
          <img src={jogador.image} alt={`Imagem de ${jogador.name}`} />
          <h2>{jogador.name}</h2>
          <p>{jogador.description}</p>
          <a href={jogador.link} class="btn">Saiba mais</a>
        </li>
      {/each}
    </ul>
    <a href="/" class="btn">Voltar para a Página Inicial</a>
  </main>
  
  <style>
    main {
      margin: 2rem;
      text-align: center;
    }
    ul {
      list-style: none;
      padding: 0;
    }
    li {
      margin-bottom: 2rem;
      text-align: center;
    }
    img {
      max-width: 80%;
      height: auto;
      border-radius: 10px;
      margin: 0 auto 1rem;
      display: block;
    }
    .btn {
      display: inline-block;
      padding: 10px 20px;
      background-color: #008CBA;
      color: white;
      text-decoration: none;
      border-radius: 5px;
    }
  </style>
  