<script lang="ts">
import Header from './Header.svelte';
import Footer from './Footer.svelte';

import 'aos/dist/aos.css';
// @ts-ignore
import AOS from "aos";




import { onMount } from 'svelte';

onMount(() => {
   AOS.init();


});





let contentTitle : string = 'My portfolio - Thierry allou kouadion juste';  
</script>


<svelte:head>
	<title>{contentTitle}</title>
</svelte:head>

<body data-scroll-container>
<Header />

<slot/>

<Footer />
</body>


<style lang="scss">
    
:global(body) {
  margin: 0 auto; /* Centrer le corps horizontalement */
  max-width: 3000px;
  background-color: #FBF7FE;
  overflow-x: hidden;
 
}
:global(html){
  scroll-behavior: smooth;
}
</style>