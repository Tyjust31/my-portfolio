<script lang="ts">
  import src from "$lib/Golap.svg";
  // Importe l'élément de ton config.scss
  let y : number = 0;

  let alt: string = "the portfolio logo"; // Description de l'image
  let aria: string = "the portfolio logo image color purple and pink"; // Description de l'image
</script>

<svelte:window bind:scrollY={y} />
{#if y > 0}
  <nav>
    <ul>
      <li>
        <img class="glass-logo" {src} {alt} aria-label={aria} />
      </li>
    </ul>
  </nav>
{:else}
  <nav>
    <ul>
      <li>
        <img {src} {alt} aria-label={aria} />
      </li>
    </ul>
  </nav>
{/if}



<style lang="scss">
  @use "$lib/configue" as *;
  @use "$lib/mixin" as *;
  @use "$lib/variable" as *;


  nav {
    @extend %div-center; /* Centre le contenu de la nav use avec configue */
    
    li {
      height: $size-logo ;
      cursor: pointer;
       
      img{
          width: $size-logo * 2; 
           margin-bottom: -70px; 

           &.glass-logo{
          @include glass-logo(255, 10px, 0.5);
         transition: all 5.5s ease-in-out;
         width: $size-logo * 2; 
         

       }
      }
    }
    ul{
       z-index: 9999;
       position: fixed;
      
      
    }
     
  }
</style>


