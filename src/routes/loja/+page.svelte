<script>
  let shirts = [
    { 
      name: "Camisa Brasil 2024", 
      image: "camisa.jpg", 
      price: "R$ 149,90", 
      link: "https://www.nike.com.br/camisa-nike-brasil-i-2023-24-jogadora-feminina-025782.html?cor=0L&utm_source=Yahoopatrocinado&utm_medium=cpc&utm_campaign=AllProducts_FP&msclkid=26a2d819c8db1a9796b4bfbbb9c64a2d" 
    },
    { 
      name: "Camisa Estados Unidos 2024", 
      image: "camisa2.jpg", 
      price: "R$ 159,90", 
      link: "https://www.centauro.com.br/camisa-nike-estados-unidos-ii-2024-25-torcedor-pro-masculina-m14ci1-mktp.html?cor=04&gad_source=1&gclid=Cj0KCQiAkoe9BhDYARIsAH85cDOt-Czh6Hn9QFsOctXEno1lhLR-DGcpw9FFFEZfRHrVHD-ljXRWmcMaAnOUEALw_wcB" 
    },
    { 
      name: "Camisa China 2024", 
      image: "camisa9.jpg", 
      price: "R$ 139,90", 
      link: "https://www.nike.com.br/camisa-nike-china-i-2023-24-torcedora-pro-feminina-026361.html?cor=P1&utm_source=Yahoopatrocinado&utm_medium=cpc&utm_campaign=AllProducts_FP&msclkid=ecce64f18bc81efb6e310353f9edbdc4" 
    }
  ];

  let volleyballs = [
    { 
      name: "Bola Oficial Mikasa V200W", 
      image: "bola.jpg", 
      price: "R$ 299,90", 
      link: "https://www.magazineluiza.com.br/bola-oficial-de-voleibol-mikasa-v200w/p/ke23b0af67/es/bldv/?utm_source=bing&utm_medium=cpc&utm_campaign=bing_eco_per_ven_sho_all_sor_3p_all-products-std&partner_id=77025&utm_term=77025&gclid=dd1425a8ab431a325982420ad9cfe223&gclsrc=3p.ds&msclkid=dd1425a8ab431a325982420ad9cfe223" 
    },
    { 
      name: "Bola de Treinamento Penalty", 
      image: "bola9.jpg", 
      price: "R$ 199,90", 
      link: "https://produto.mercadolivre.com.br/MLB-908323468-bola-de-volei-penalty-mg-3600-soft-oficial-volley-promoco-_JM?matt_tool=59082313&matt_word=&matt_source=bing&matt_campaign=MLB_ML_BING_AO_APP%20%26%20SPORTS-ALL-ALL_X_PLA_ALLB_TXS_ALL&matt_campaign_id=382858293&matt_ad_group=APP%20%26%20SPORTS&matt_match_type=e&matt_network=o&matt_device=c&matt_keyword=default&msclkid=89266db46329135f371c0a161199c39e&utm_source=bing&utm_medium=cpc&utm_campaign=MLB_ML_BING_AO_APP%20%26%20SPORTS-ALL-ALL_X_PLA_ALLB_TXS_ALL&utm_term=4581252654962603&utm_content=APP%20%26%20SPORTS" 
    },
    { 
      name: "Bola Olímpica 2024 Especial", 
      image: "bola6.jpg", 
      price: "R$ 349,90", 
      link: "https://www.google.com/imgres?q=produto%20nao%20disponivel%20imagem%20escrito%20isso&imgurl=https%3A%2F%2Fwww.herbicat.com.br%2Fimagens%2Fuploads%2Fproduto%2F207%2Fimg%2Ftbd_20160405092922oalHJWV8z.jpg&imgrefurl=https%3A%2F%2Fwww.herbicat.com.br%2Fproduto%2Fponta-teejet-visiflo-inox-com-inducao-de-ar-aiub.html&docid=YOG9U1jl_wV7UM&tbnid=PWaewoxnYPpOOM&vet=12ahUKEwib2IyB6aqLAxVcgGEGHZXCNpIQM3oECBkQAA..i&w=625&h=625&hcb=2&ved=2ahUKEwib2IyB6aqLAxVcgGEGHZXCNpIQM3oECBkQAA" 
    }
  ];
</script>

<main>
  <h1>Loja de Produtos</h1>

  <h2>Camisas Olímpicas</h2>
  <ul class="products">
    {#each shirts as shirt}
      <li>
        <img src={shirt.image} alt={`Imagem de ${shirt.name}`} />
        <h2>{shirt.name}</h2>
        <p>{shirt.price}</p>
        <a href={shirt.link} target="_blank" class="btn">Comprar</a>
      </li>
    {/each}
  </ul>

  <h2>Bolas de Vôlei</h2>
  <ul class="products">
    {#each volleyballs as ball}
      <li>
        <img src={ball.image} alt={`Imagem de ${ball.name}`} />
        <h2>{ball.name}</h2>
        <p>{ball.price}</p>
        <a href={ball.link} target="_blank" class="btn">Comprar</a>
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
  h1, h2 {
    color: #333;
  }
  .products {
    list-style: none;
    padding: 0;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 2rem;
  }
  li {
    max-width: 200px;
    text-align: center;
  }
  img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
  }
  .btn {
    display: inline-block;
    padding: 10px 20px;
    background-color: #ff6b6b;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 10px;
  }
</style>