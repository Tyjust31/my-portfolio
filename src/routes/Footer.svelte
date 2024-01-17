<script lang="ts">
  import google from "$lib/googel.svg";
  import fb from "$lib/facebook.svg";
  import lin from "$lib/lin.svg";
  import x from "$lib/x.svg";
  import insta from "$lib/instagram.svg"
 

  interface Reseau {
    src: string;
    alt: string;
    href?: string;
  }

  let name: Reseau[] = [
    { src: google, alt: "logo googel", href: "https://google.com" },
    { src: fb, alt: "logo facebook", href: "https://facebook.com" },  
    { src: lin, alt: "logo linkdin", href: "https://linkedin.com" },
    { src: x, alt: "logo x", href: "https://twitter.com/Tyjust31" },
    { src: insta, alt: "logo intagramz", href: "https://www.instagram.com/tyjust31/" }
  ];
</script>


  
<main>
  <h4 data-aos="fade-down"  data-aos-duration="1000">Contact</h4>
  <div class="reseau">
    {#each name as { src, alt, href }}
      {#if typeof href === "string"}
        <a data-aos="fade-up"  data-aos-duration="500" {href}><img {src} {alt} /></a>
      {:else}
        <img {src} {alt} />
      {/if}
    {/each}
  </div>

  <h3  >
    Designed and built by 'Juste ALLOU'
    <span>&copy; Copyright 2024 - Juste ALLOU</span>
  </h3>

  <hr />
  </main>
  
  <style lang="scss">
    @use "$lib/variable" as *;
  
    main {
      h4 {
        margin-top: 50px;
        text-align: center;
        font-size: $size-text * 3 / 2;
        font-family: $second-font;
        font-weight: 300;
        color: $texte;
      }
  
      .reseau {
        display: grid;
      grid-template-columns: repeat(5, 1fr);
      grid-template-rows: repeat(5, 1fr);
      grid-gap: 10px;
        place-items: center;
        justify-content: center;
        align-items: center;
      }
  
      h3 {
        font-family: $first-font;
        font-size: $size-text * 2;
        max-width: 70%;
        margin-left: 20%;
        margin-top: -350px;
      }
    }
    @media only screen and (max-width: 640px) {


main {
      h4 {
        margin-top: 50px;
        text-align: center;
        font-size: 3em;
        font-family: $second-font;
        font-weight: 300;
        color: $texte;
      }
  
      .reseau {
       
       display: flex;
       flex-direction: column;
        
      }
  
      h3 {
        
        font-size: 3em;
        max-width: 70%;
        margin-left: 20%;
        margin-top: 30px;
      }
    }
    a{
      font-size: 3em;
    }
}
  </style>
  