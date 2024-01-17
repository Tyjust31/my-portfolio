<script lang="ts">
    
  // import arriere from '$lib/arriere-plan.jpg';

  import moi from "$lib/moi-min-min.webp";
  import fondc from "$lib/fondc-min.webp"
  //import fond from "$lib/fond.jpg";
  let alt: string = "photo de moi";

  export let y: number = 0;
 

</script>






<svelte:window bind:scrollY={y} />

<body>
  

{#if y < 200}
  <main
    aria-current="page"
    style="background: url('{fondc}') no-repeat center ; background-size: cover;"
  >
    <section>
      <div class="trait" aria-label="ligne"></div>
      <br />

     
      <h1  data-aos="zoom-in-down" data-aos-once="true" 
      aria-label="title i am tyjust" 
      >I am tyjust</h1>
     

      <img src={moi} {alt} />
      <h2 >tech Software </h2>
      <h3>Developer & Designer</h3>
      <div class="traite"></div>
    </section>
  </main>
{:else if y > 200 && y < 400}
  <main
    style="background: url('{fondc}') no-repeat center ;  background-size: cover; "
  >
    <main
      aria-current="page"
      style="background: url('{fondc}') no-repeat center ; background-size: cover;"
    >
      <section>
        <div class="trait" aria-label="ligne"></div>
        <br />
        <h1 aria-label="title i am tyjust">I am tyjust</h1>
        <img src={moi} {alt} />
        <h2> tech lover❤️</h2>
        <h3>Developer & Designer</h3>
        <div class="traite"></div>
      </section>
    </main>
  </main>
{:else if y > 400}
  <main
    aria-current="page"
    style="background: url('{fondc}') no-repeat center ; background-size: cover;"
  >
    <section>
      <div class="trait" aria-label="ligne"></div>
      <br />
      <h1 aria-label="title i am tyjust">I am tyjust</h1>
      <img src={moi} {alt} />
      <h2 >i'm the best 😝</h2>
      <h3>Developer & Designer</h3>
      <div class="traite"></div>
    </section>
  </main>
{/if}

</body>

<style lang="scss">
  @use "$lib/configue" as *;
  @use "$lib/mixin" as *;

 
    main {
      height: 130vh;
      width: 100vw;
      section {
        @include glass-logo(255, 10px, 0.1);
        position: absolute;
        top: 65%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        height: 110%;

        

        .trait {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 25px;
          position: absolute;
          margin-left: 30%;
        }

        .traite {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 10px;
          position: absolute;
          margin-left: 30%;
        }

        h1 {
          @extend %text-conf;
        }
         img{
          @extend %div-center;
          margin-left: 43%;
          width: 14%;
          border-radius: 50px;
          box-shadow: 0 0 0 0;
          border: 10px solid rgba(222, 232, 249, 0.312);
          cursor: progress;
          transition: ease-in-out 3s ;
          &:hover{
            transform: scale(1.2);
            
          }
    
         }
        h2 {
          @extend %text-confe;
        }

        h3 {
          @extend %text-confeg;
        }
      }
    }
    @media only screen and (max-width: 420px) {
  main {
      height: 140vh;
      width: 100vw;
      section {
      
        top: 70%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        height: 110%;

        

        .trait {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 25px;
          position: absolute;
          margin-left: 30%;
        }

        .traite {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 10px;
          position: absolute;
          margin-left: 30%;
        }

        h1 {
         text-align: center;
         font-size: calc(3em * 1.5) ;

        }
         img{
         
          margin-left: 43%;
          width: 14%;
          border-radius: 50px;
          box-shadow: 0 0 0 0;
          border: 10px solid rgb(192, 191, 255);
          cursor: progress;
          transition: ease-in-out 3s ;
          &:hover{
            transform: scale(1.2);
            
          }
    
         }
        h2 {
          text-align: center ;
          font-size: 0.5em ;
        }

        h3 {
          font-size: 1.8em;
        }
      }
    }
}

    @media only screen and (max-width: 430px) {
  main {
      height: 140vh;
      width: 100vw;
      section {
      
        top: 70%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        height: 110%;

        

        .trait {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 25px;
          position: absolute;
          margin-left: 30%;
        }

        .traite {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 10px;
          position: absolute;
          margin-left: 30%;
        }

        h1 {
         text-align: center ;
         font-size: calc(3em * 1.6) ;

        }
         img{
         
          margin-left: 43%;
          width: 14%;
          border-radius: 50px;
          box-shadow: 0 0 0 0;
          border: 10px solid rgb(192, 191, 255);
          cursor: progress;
          transition: ease-in-out 3s ;
          &:hover{
            transform: scale(1.2);
            
          }
    
         }
        h2 {
          text-align: center ;
          font-size: 0.5em ;
        }

        h3 {
          font-size: 1.8em;
        }
      }
    }
}

/* Pour les écrans jusqu'à 600 pixels de large (par exemple, smartphones) */
@media only screen and (max-width: 620px) {
  main {
      height: 140vh;
      width: 100vw;
      section {
      
        top: 70%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        height: 110%;

        

        .trait {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 25px;
          position: absolute;
          margin-left: 30%;
        }

        .traite {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 10px;
          position: absolute;
          margin-left: 30%;
        }

        h1 {
         text-align: center;
         font-size: calc(3em ) 
         
        }
         img{
         
          margin-left: 43%;
          width: 44%  !important;
          border-radius: 50px;
          box-shadow: 0 0 0 0;
          border: 10px solid rgb(192, 191, 255);
          cursor: progress;
          transition: ease-in-out 3s ;
          &:hover{
            transform: scale(1.2);
            
          }
    
         }
        h2 {
          text-align: center ;
          font-size: calc(3em * 1.1) ;
        }

        h3 {
          font-size: 1.8em;
        }
      }
    }
}

/* Pour les écrans jusqu'à 768 pixels de large (par exemple, tablettes en mode portrait) */
@media only screen and (max-width: 768px) {
  main {
      height: 140vh;
      width: 100vw;
      section {
      
        top: 70%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        height: 110%;

        

        .trait {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 25px;
          position: absolute;
          margin-left: 30%;
        }

        .traite {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 10px;
          position: absolute;
          margin-left: 30%;
        }

        h1 {
         font-size: calc(3em * 1.5)  !important;
        }
         img{
         
          margin-left: 43%;
          width: 14%;
          border-radius: 50px;
          box-shadow: 0 0 0 0;
          border: 10px solid rgb(192, 191, 255);
          cursor: progress;
          transition: ease-in-out 3s ;
          &:hover{
            transform: scale(1.2);
            
          }
    
         }
        h2 {
          font-size: calc(3em * 1.20) !important ;
          text-align: center;
          margin-left: -2% ;
        }

        h3 {
          font-size: 1.8em;
          margin-top: 10px;
        }
      }
    }
}

/* Pour les écrans jusqu'à 1024 pixels de large (par exemple, tablettes en mode paysage) */
@media only screen and (max-width: 1024px) {
  h1 {
   
    font-size: 1em;
    
    
  }
}

/* Pour les écrans jusqu'à 1440 pixels de large (par exemple, ordinateurs portables) */
@media only screen and (max-width: 1520px) {
  main {
      height: 140vh;
      width: 100vw;
      section {
      
        top: 65%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        height: 110%;

        

        .trait {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 25px;
          position: absolute;
          margin-left: 30%;
        }

        .traite {
          width: 40%;
          height: 1px;
          background-color: black;
          margin-top: 10px;
          position: absolute;
          margin-left: 30%;
        }

        h1 {
         font-size: calc(3em * 2.5);
        }
         img{
         
          margin-left: 43%;
          width: 14%;
          border-radius: 50px;
          box-shadow: 0 0 0 0;
          border: 10px solid rgb(241, 241, 244);
          cursor: progress;
          transition: ease-in-out 3s ;
          &:hover{
            transform: scale(1.2);
            
          }
    
         }
        h2 {
          font-size: calc(3em * 2);
        }

       
      }
    }
}

</style>






