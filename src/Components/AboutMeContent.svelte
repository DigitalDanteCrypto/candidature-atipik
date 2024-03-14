<script>
  import ImageContent from "./ImageContent.svelte";
  import me from '../assets/me.jpg';

</script>

<div id="aboutme">
    <h3>En tant que junior développeur fullstack, qu'est-ce que tu préfères dans ce domaine ?</h3>
  <p>
    Ayant récemment fini mes études, il me reste encore pleins de choses à découvrir. 
    Il faut savoir qu'au début, la programmation et moi n'étions pas ami, venant d'un background plus créatif et libre
    en matière de conception comme la production musicale, mon apprentissage dans la programmation fut rude.
    J'ai passer de nombreux cours à distance à cause du COVID et de nombreuse nuit à me tirer les cheveux sur les différents
    conceptes de développement. Cependant la programmation ma appris une chose très rapidement, c'est trouver des solutions et vite,
    que se soit pour un bug de dernière minutes avant une présentation ou implémenter une logique qui est en dehors de mon niveau. J'ai appris à
    réduire mon problème au maximum pour en tirer une solution simple. Pour moi, le code doit être simple et lisible. Quitte a rajouter une ligne ou deux.


  </p>
  <blockquote>
    <svg class="quotty" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 18 14">
        <path d="M6 0H2a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3H2a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Zm10 0h-4a2 2 0 0 0-2 2v4a2 2 0 0 0 2 2h4v1a3 3 0 0 1-3 3h-1a1 1 0 0 0 0 2h1a5.006 5.006 0 0 0 5-5V2a2 2 0 0 0-2-2Z"/>
    </svg>
    <p>You should name a variable using the same care with which you name a first-born child.</p>
   <footer>— Robert C. Martin</footer>
  </blockquote>
  
  <p id="bottom-paragraph">
    <br />
    Mon quotidien est rythmé par deux choses : mon envie inépuisable d'apprendre dans plein de domaines différents et la salle de sport. 
    J'essaie de mener une vie active tout en passant la plupart de mes journées à coder des projets. Un jour je peux passer 8h d'affilée à essayer de reverse
    engineering un jeu-vidéo des années 2000 et le lendemain mettre la même énergie pour créer une scène sur 3D Blender.  Le week-end je sors faire de la photographie
    et  parfois je suis appeler à photographier des groupes de musiques en passage à Genève pour un concert.
    Mais le plus important pour moi c'est de pratiqué la programmation tout les jours. J'ai appris les pluparts des matières en auto-didacte, en suivant
    des explications sur youtube et m'exercant dans mon coin. Je touche vraiment à tout, un peu trop même. Mais c'est ce qui me plaît et qui me donne envie d'avancer et de progresser.
    J'adore aussi transmettre mes connaissances, ce que je sais et mes expériences. C'est pour cela que je donne cours chez CodeCamp Switzerland pendant les vacances scolaire aux enfants.
    Il n'y a pour moi rien de plus satisfaisant que de transmettre de la connaissances à quelqu'un.  
  </p>
  <ImageContent src={me} />
</div>

<style>

blockquote, #aboutme {
  font-family: "Inter", sans-serif;
}

.quotty {
  width: 2vw;
  height: 2vh;
  color: orange;
}

h3 {
  color: rgba(38, 43, 56, 0.856);
  line-height: 2;
  font-weight: 600;
}

p {
  font-weight: 400;
  line-height: 1.75rem;
  text-align: justify;
}

blockquote {
  font-weight: 600;
  margin: 0;
  padding: 40px;
}

blockquote p {
  padding: 1.5rem;
  --pipou-bg-opacity: 1;
  background-color: rgb(229 231 235 / var(--pipou-bg-opacity));
  border-radius: 5px;
  content: '\201C'; /* Moved here as an initial style, but it needs to be within a pseudo-element */
}

blockquote p::before {
  content: '\201C';
}

blockquote p::after {
  content: '\201D';
}

#bottom-paragraph {
  margin-bottom: 4rem;
}

/* MOBILE */
@media screen and (min-width: 320px) {
  #aboutme {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-left: 2rem;
    padding-right: 2rem;
  }
}

/* DESKTOP */
@media screen and (min-width: 1024px) {
  #aboutme {
    padding-left: 8rem;
    padding-right: 8rem;
  }
}
</style>
