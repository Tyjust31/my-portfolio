
<script>
  import portfolio from '$lib/portfolio1-min-min.webp'
  import portfolioo from '$lib/portfolio2-min.webp'
  import portfoliooo from '$lib/portfolio3-min.webp'
</script>

<main>

    <h4 data-aos="fade-down" data-scroll data-scroll-speed="1"  data-aos-duration="1000">project</h4>
    <div class="competence">
    <div class="competencea">
    <img  data-aos-duration="2500"   data-aos-delay="80" data-aos-easing="ease-in-out" data-aos="fade-up-left" src={portfolio} width="70%" style="cursor: pointer;" alt="portfolio 1" >
  </div>
  <div class="competenceb">
    <img  data-aos-duration="2500"   data-aos-delay="50" data-aos="fade-up-right"  data-aos-easing="ease-in-out" src={portfolioo} width="130%" style="cursor: pointer;" alt="portfolio 2">
  </div>
  <div class="competencea">
    <img  data-aos-duration="2500"    data-aos-delay="50" data-aos-easing="ease-in-out" data-aos="fade-up-left" src={portfoliooo} width="70%" style="cursor: pointer;" alt="portfolio 3">
  </div>
</div>
<hr>
<h3>create our onw world everythig is possible keep going to believe</h3>
       <hr>
</main>



<style lang="scss">
    
    @use "$lib/mixin" as *;
    @use "$lib/configue" as *;
    
  
    main {
      background: rgb(255,255,255);
background: linear-gradient(0deg, #fbf7fe 11%,#0f63c3 18%, #fbf7fe 74%);

      width: 100%;
      h4 {
        margin-top: 50px;
        text-align: center;
        font-size: $size-text * 1.5;
        font-family: $second-font;
        color: rgba(0, 0, 0, 0.8);
      }
      h3{
          font-size: $size-text * 2 ;
          font-family: $first-font;
          color: rgba(0, 0, 0, 0.8);
      }
      .competence{
    
        .competencea{
          margin-left: 5%;
          transition: 2s ease-in-out ;
          &:hover{
          transform: translateX(350px);
          transition: 2s ease-in-out ;
        }
        }
        
        .competenceb{
          margin-left: 40%;
          transition: 2s ease-in-out ;
          &:hover{
          transform: translateX(-350px);
          transition: 2s ease-in-out ;
        }
        }
        
      }
    }
    @media only screen and (max-width: 640px) {



      main {
      background: rgb(255,255,255);
background: linear-gradient(0deg, #fbf7fe 11%,#0f63c3 18%, #fbf7fe 74%);

      width: 100%;
      h4 {
        margin-top: 50px;
        text-align: center;
        font-size: 3em;
        font-family: $second-font;
        color: rgba(0, 0, 0, 0.8);
      }
      h3{
          font-size: 3em ;
          font-family: $first-font;
          color: rgba(0, 0, 0, 0.8);
      }
      .competence{
    
        .competencea{
          margin-left: 5%;
          transition: 2s ease-in-out ;
          &:hover{
          transform: translateX(350px);
          transition: 2s ease-in-out ;
        }
        }
        
        .competenceb{
          margin-left: 40%;
          transition: 2s ease-in-out ;
          &:hover{
          transform: translateX(-350px);
          transition: 2s ease-in-out ;
        }
        }
        
      }
    }

}
  </style>