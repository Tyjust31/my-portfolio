
<script lang="ts">
  export let y: number = 0;
  import sql from "$lib/sql.svg";
  import svelt from "$lib/svelte-min-min.svg";
  import supabase from "$lib/supabase.svg";
  import typescript from "$lib/typescript.svg";
  import zig from "$lib/zig.svg";
  import jslogo from "$lib/js.svg";
  import astro from "$lib/astro.svg";
  import next from "$lib/next.svg";
  import bun from "$lib/bun.svg";
  import nodejs from "$lib/node.svg";
  import figma from "$lib/figma.svg";
  import canva from "$lib/canva.svg";
  import github from "$lib/github.svg";
  import { fade } from "svelte/transition"; 
  
  // J'ai remplacé le code sélectionné comme demandé

</script>

<svelte:window bind:scrollY={y}/>
<body>
  

{#if y > 1700 && y < 3400   }

<main in:fade={{duration:500}} out:fade={{duration:500}}  style="background: rgba(0, 0, 0, 0.9) ; " >

  <h4  class="dark" data-aos="fade-up"  data-aos-duration="2000">competence</h4>
  <div class="competence dark">
  <div class="competencea">
  <p style="font-size: 100px"   class="dark">front end</p> <br>
  <p  data-aos="fade-right"  data-aos-duration="500"> <img src={typescript} width="60px" alt="">typescript</p> 
  <p data-aos="fade-right"  data-aos-duration="500">  <img src={svelt} width="60px" alt="">svelte</p> 
  <p data-aos="fade-right"  data-aos-duration="500">  <img src={jslogo} width="60px" alt="">javascript</p> 
  <p data-aos="fade-right"  data-aos-duration="500">  <img src={astro} width="60px" alt="">astro</p> 
  <p data-aos="fade-right"  data-aos-duration="500">  <img src={next} width="60px" alt="">next</p> 
</div>
<div class="competenceb dark">
  <p  style="font-size: 100px" >backend</p> <br>
 <p data-aos="fade-left"  data-aos-duration="500">  <img src={sql} width="60px" alt="">postgresql</p> 
 <p data-aos="fade-left"  data-aos-duration="500">  <img src={supabase} width="60px" alt="">supabase</p>  
 <p data-aos="fade-left"  data-aos-duration="500">  <img src={bun} width="60px" alt="">bun</p> 
 <p data-aos="fade-left"  data-aos-duration="500">  <img src={nodejs} width="60px" alt="">node js</p> 
  <p data-aos="fade-left"  data-aos-duration="500">  <img src={zig} width="60px" alt="">zig</p> 
</div>
<div class="competencea dark">
  <p style="font-size: 100px" >tools</p> <br>
  <p data-aos="fade-right"  data-aos-duration="500">  <img src={figma} width="30px" alt="">figma</p> 
  <p data-aos="fade-right"  data-aos-duration="500">  <img src={canva} width="60px" alt="">canva</p>  
  <p data-aos="fade-right"  data-aos-duration="500">  <img src={github} width="60px" alt="">github</p>  
</div>
</div>
         
<hr>
<h3 style="color: aliceblue;">
  evething is possible you can do everything keep going to belive
</h3>
<hr>
      
</main>



{:else}
  <main>
    <h4 data-aos="fade-down"  data-aos-duration="2000">competence</h4>
    <div class="competence">
      <div class="competencea">
        <p style="font-size: 100px" >front end</p> <br>
        <p>  <img src={typescript} width="60px" alt="">typescript</p> 
        <p>  <img src={svelt} width="60px" alt="">svelte</p> 
        <p>  <img src={jslogo} width="60px" alt="">javascript</p> 
        <p>  <img src={astro} width="60px" alt="">astro</p> 
        <p>  <img src={next} width="60px" alt="">next</p> 
      </div>
      <div class="competenceb">
        <p style="font-size: 100px" >backend</p> <br>
 <p>  <img src={sql} width="60px" alt="">postgresql</p> 
 <p>  <img src={supabase} width="60px" alt="">supabase</p>  
 <p>  <img src={bun} width="60px" alt="">bun</p> 
 <p>  <img src={nodejs} width="60px" alt="">node js</p> 
  <p>  <img src={zig} width="60px" alt="">zig</p>
      </div>
      <div class="competencea">
        <p style="font-size: 100px" >tools</p> <br>
        <p  data-aos-duration="1500" data-aos="fade-right">  <img src={figma} width="30px" alt="">figma</p> 
        <p  data-aos-duration="1500" data-aos="fade-right">   <img src={canva} width="60px" alt="">canva</p>  
        <p   data-aos-duration="1500" data-aos="fade-right">  <img src={github} width="60px" alt="">github</p>  
      </div>
    </div>

    <hr />
    <h3 style="color: black;">
        evething is possible you can do everything keep going to belive
      </h3>
    <hr />
  </main>
{/if}
</body>
<style lang="scss">
    
    @use "$lib/mixin" as *;
    @use "$lib/configue" as *;
  
    main {
      width: 100%;
      transition: 3s ease-in-out;
      h4 {
        margin-top: 50px;
        text-align: center;
        font-size: $size-text * 1.5;
        font-family: $second-font;
        &.dark {
          color: aliceblue;
        }
      }
      p {
        
        font-size: $size-text;
        font-family: $three-font;
      }
      h3{
          font-size: $size-text * 2 ;
          font-family: $first-font;
      }
      .competence{
        &.dark{
            color: aliceblue;
          }
        .competencea{
          margin-left: 20%;
          
        }
        .competenceb{
          margin-left: 60%;
        }
        
      }
    }

    @media only screen and (max-width: 640px) {

main {
width: 100%;
transition: 3s ease-in-out;
h4 {
  margin-top: 50px;
  text-align: center;
  font-size: 2.5em;
  
  &.dark {
    color: aliceblue;
  }
}
p {
  
  font-size: 2.5em;
 
}
h3{
    font-size: 2.5em ;
    
}
.competence{
  &.dark{
      color: aliceblue;
    }
  .competencea{
    margin-left: 20%;
    
  }
  .competenceb{
    margin-left: 30% !important;
  }
  
}
}
}

    @media only screen and (max-width: 1440px) {

      main {
      width: 100%;
      transition: 3s ease-in-out;
      h4 {
        margin-top: 50px;
        text-align: center;
        font-size: 2.5em;
        
        &.dark {
          color: aliceblue;
        }
      }
      p {
        
        font-size: 2.5em;
       
      }
      h3{
          font-size: 2.5em ;
          
      }
      .competence{
        &.dark{
            color: aliceblue;
          }
        .competencea{
          margin-left: 20%;
          
        }
        .competenceb{
          margin-left: 60%;
        }
        
      }
    }
    }
</style>
  