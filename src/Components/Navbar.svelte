<script>
  import { onMount } from "svelte";
  

  let scrollPosition = 0;

  function updateScrollPosition() {
    scrollPosition = window.scrollY;
  }

  onMount(() => {
    window.addEventListener("scroll", updateScrollPosition);

    return () => {
      window.removeEventListener("scroll", updateScrollPosition);
    };
  });

  // Reactive statement for dynamic navbar padding
  $: navbarPaddingTop = scrollPosition === 0 ? "30px" : "20px";
</script>

<nav style="padding-top: {navbarPaddingTop};">
  <p class="logo">Florian Secretan</p>
  <a href="#aboutme">A propos de moi</a>
  <a href="#myprojects">Mes projets</a>
  <a href="#motivations">Motivations</a>
  <a href="https://www.swisstransfer.com/d/e3c16043-d5d9-43cc-896e-58922f774c30" target="_blank">Dossier Candidature</a>
  <button class="contact-btn">Contact</button>
</nav>

<style>
/* MOBILE */

@media screen and (min-width: 320px){
  nav {
    font-family: "Inter", sans-serif;
    display: flex;
    justify-content: space-between;
    padding: 20px;
    align-items: center;
    margin-left: auto;
    margin-right: auto;
    padding-left: 2rem;
    padding-right: 2rem;
    position: -webkit-sticky; /* For Safari */
    position: sticky;
    top: 0;
    z-index: 1000;
    backdrop-filter: blur(2px);
    transition: padding-top 0.2s ease-in-out;
  }

  nav .logo {
    margin-right:1rem;
    font-weight: 700;
    font-size: 24px;
    background: linear-gradient(135deg, #ff5339 34.37%, #2ad4ff);
    -webkit-text-fill-color: transparent;
    /* OUI j'ai piqué le code désolé */
    animation: gradient 1s linear infinite;
    background-color: rgba(0, 0, 0, 0);
    background-position-x: 0%;
    background-position-y: 0%;
    background-repeat: repeat;
    background-attachment: scroll;
    background-image: linear-gradient(
      135deg,
      rgb(255, 83, 57) 54.27%,
      rgb(236, 147, 30)
    );
    background-clip: text;
    background-size: 100% 100%;
    clip-path: inset(1px);
  }

  nav a {
    display:none;
    text-decoration: none;
    color: #333;
    margin: 0 10px;
  }

  nav a:hover {
    color: #666;
  }

  .contact-btn {
    font-family: "Inter", sans-serif;
    color: white;
    background-color: #ed6a0c;
    border: none;
    padding: 10px 20px;
    border-radius: 20px;
    cursor: pointer;
    transition:
      background-color 0.3s,
      box-shadow 0.3s;
  }

  .contact-btn:hover {
    background-color: darkorange;
    box-shadow: 0 0 8px 4px rgba(255, 165, 0, 0.6);
  }

}




/* DESKTOP */

@media screen and (min-width: 1024px){



  nav {
    font-family: "Inter", sans-serif;
    width: 70%;
    display: flex;
    justify-content: space-between;
    padding: 20px;
    align-items: center;
    margin-left: auto;
    margin-right: auto;
    padding-left: 2rem;
    padding-right: 2rem;
    position: -webkit-sticky; /* For Safari */
    position: sticky;
    top: 0;
    z-index: 1000;
    backdrop-filter: blur(2px);
    transition: padding-top 0.2s ease-in-out;
  }

  nav .logo {
    font-weight: 700;
    font-size: 24px;
    background: linear-gradient(135deg, #ff5339 34.37%, #2ad4ff);
    -webkit-text-fill-color: transparent;
    /* OUI j'ai piqué le code désolé */
    animation: gradient 1s linear infinite;
    background-color: rgba(0, 0, 0, 0);
    background-position-x: 0%;
    background-position-y: 0%;
    background-repeat: repeat;
    background-attachment: scroll;
    background-image: linear-gradient(
      135deg,
      rgb(255, 83, 57) 54.27%,
      rgb(236, 147, 30)
    );
    background-clip: text;
    background-size: 100% 100%;
    clip-path: inset(1px);
  }

  nav a {
    display:flex;
    text-decoration: none;
    color: #333;
    margin: 0 10px;
  }

  nav a:hover {
    color: #666;
  }

  .contact-btn {
    font-family: "Inter", sans-serif;
    color: white;
    background-color: #ed6a0c;
    border: none;
    padding: 10px 20px;
    border-radius: 20px;
    cursor: pointer;
    transition:
      background-color 0.3s,
      box-shadow 0.3s;
  }

  .contact-btn:hover {
    background-color: darkorange;
    box-shadow: 0 0 8px 4px rgba(255, 165, 0, 0.6);
  }
}
</style>
