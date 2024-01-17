<script lang="ts">



</script>

<main >

    <h4  data-aos="fade-up" data-aos-duration="1000">about me</h4>
    <p data-aos="fade-down" data-aos-duration="2000">my name is juste allou  founder and ceo Tech <br>
        i love tech create is my life front end ux/ui <br>
        and backend i love create software  i’m <br>
        raiser in ivoiry coast and i believe about<br> 
        human competence and every body can succed<br>
               
        <hr>
 <h3>create our onw world everythig is possible keep going to believe</h3>
</main>




<style lang="scss">
  @use "$lib/variable" as *;
  @use "$lib/mixin" as *;
  @use "$lib/variable" as *;
  main {
    background: rgb(251,247,254);
background: linear-gradient(0deg, rgba(251,247,254,1) 25%, rgba(142,159,240,1) 70%, rgba(251,247,254,1) 97%);
    width: 100%;
    h4 {
      margin-top: 50px;
      text-align: center;
      font-size: $size-text * 1.5;
      font-family: $second-font;
      font-weight: 300;
      color: $texte;
      
    }
    p {
      text-align: center;
      font-size: $size-text;
      font-family: $three-font;
      color: $texte;
    }
    h3{
        font-size: $size-text * 1.6 ;
        font-family: $first-font;
        color: $texte;
    }
  }



/* Pour les écrans jusqu'à 1440 pixels de large (par exemple, ordinateurs portables) */
@media only screen and (max-width: 1440px) {
  main {
    background: rgb(251,247,254);
background: linear-gradient(0deg, rgba(251,247,254,1) 25%, rgba(142,159,240,1) 70%, rgba(251,247,254,1) 97%);
    width: 100%;
    h4 {
      margin-top: 50px;
      text-align: center;
      font-size: 3em;
      
    }
    p {
      text-align: center;
      font-size: 2.4em ;
     
    }
    h3{
        font-size: 3em ;
       
    }
  }
}
</style>

