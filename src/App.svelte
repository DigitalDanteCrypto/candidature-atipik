<script>
  import AboutMeContent from "./Components/AboutMeContent.svelte";
import ImageContent from "./Components/ImageContent.svelte";
import LeadingBanner from "./Components/LeadingBanner.svelte";
import Navbar from "./Components/Navbar.svelte";
import myself from '../src/assets/myself.jpg';
  import ProjectsContent from "./Components/ProjectsContent.svelte";
  import MotivationContent from "./Components/MotivationContent.svelte";
  import Footer from "./Components/Footer.svelte";
 
</script>
<Navbar />
<main>
  <LeadingBanner />
  <ImageContent src={myself}/>
  <AboutMeContent />
  <ProjectsContent />
  <MotivationContent />
  
  
</main>
<Footer />

<style>

/* MOBILE */

@media screen and (min-width: 320px){

  main {
    display: block;
  }

}




/* DESKTOP */

@media screen and (min-width: 1024px){
  main {
    max-width: 1280px;
    margin-left: auto;
  margin-right: auto;
  margin-top: 9rem;
    padding-left: 8rem;
    padding-right: 8rem;
  }

}


</style>
