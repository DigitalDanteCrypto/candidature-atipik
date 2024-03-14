<script>
  import ImageContent from "./ImageContent.svelte";
  import project from '../assets/myself.jpg'
  import demo_video from "../assets/demo_warthunderAPP.mp4";
  import github_logo from "../assets/github-sign.png"
  import team from "../assets/teamnft.png";
  import ecowise from "../assets/ecowise.png";

</script>

<div id="myprojects" class="reusable-style-v1">
  <h3>Parlons un peu de mes projets, qu'est ce que je sais faire ?</h3>
  <p>Voici quelques projets qui on eu le plus d'impacte dans mon apprentissage</p>
  <a id="githubimg" href="https://github.com/DigitalDanteCrypto" target="_blank"><img  src={github_logo} alt=""></a>
  <ul>
    <li><a href="https://github.com/DigitalDanteCrypto/warthunderhelper/tree/mvc">War Thunder Helper</a></li>
    <li>Restaurant Point-of-Selling</li>
    <li>Solana NFT Project</li>
    <li><a href="https://medium.com/@florian.secretan/projet-de-sp%C3%A9cialisation-data-science-5c04d80c9dae" target="_blank">Recherche Data Science (Projet universitaire)</a></li>
    <li>Prototypage Application Mobile(Mémoire Bachelor)</li>
  </ul>
  <h3>Le projet War Thunder Helper</h3>
  <p>
    L'idée de ce projet vient de mes sessions de jeu. Par exemple, en jouant à un jeu vidéo, je réfléchis à comment créer un outil pour faciliter certaines tâches. C'est ainsi qu'en jouant à War Thunder, il m'est venue l'idée de créer une interface simple d'utilisation où je regroupe les informations importantes sur les avions et les compare avec d'autres avions. Ainsi, l'utilisateur, grâce à quelques clics, peut avoir un visuel utile sur ses avantages et inconvénients, et adapter son gameplay en fonction des informations recueillies.
    <br />
    Aspect technique : <br />
    J'ai tout d'abord récupérer les informations importante sur le Wikipedia du jeu, trier les informations, crée un scraper en <u>Python</u> pour les 
    tâche répétitif, ensuite j'ai crée un script en <u>Javascript</u> pour crée le json avant de l'insérer dans ma BD sur <u>MongoDB</u>, 
    <b><a href="https://i.postimg.cc/wMDzpYJk/carbon.png" target="_blank">voici un snippet</a></b>. Pour crée l'API et le backend j'ai utiliser <u>Java</u> et <u>SpringBoot</u> c'était mon premier projet avec ces outils, j'ai trouvé intuitif et facile à comprendre la création des Routes et Controllers.
    Pour le frontend j'ai utilisé React, l'utilisation des hooks mon été utile pour gérer dynamique les données. J'y ai appris l'utilisation du useContext Hook pour manager l'état des données plus facilement à travers les différents components.
    Pour l'UI j'ai utiliser une librairie Open Source appeler <u><a href="https://mui.com/material-ui/" target="_blank">Material UI</a></u><br />
    Aspect apprentissage : <br />
    Nicolas Paschoud, Software Engineer chez Pictet et mon mentor, à jouer le rôle de Product Owner et avec lui nous avons défini une petite pipe-line et m'a expliqué le bonne pratique sur Github comme crée des branches pour chaque features, merge request, pull request , <u>faire du code review</u> et définir des ticket sur <u>Trello</u>.
    Le projet n'est pas encore disponible pour le publique mais le MVP est opérationel, il ne reste plus qu'à augmenter les données dans la base de données.

    <br />
    <b><a href="https://github.com/DigitalDanteCrypto/warthunderhelper/tree/mvc" target="_blank">Pour jeter un oeil au code..</a></b> 


  </p>
  <div id="video-frame">
    <video width="1280" height="360" autoplay muted loop>
      <source src={demo_video} type="video/mp4" />
      Your browser does not support the video tag.
    </video>
  </div>
  <h3 id="breaking-header">Le projet Restaurant Point-Of-Selling</h3>
  <p>
    Ce projet consiste à créer une application pour les tablettes dans les restaurants. Un client pourra ainsi commander ses plats depuis un appareil, et l'offre sera envoyée en temps réel et accessible depuis un panneau d'administration. Pour ce projet, j'ai décidé de partir sur la création d'une base de données relationnelle avec <u>PostgreSQL</u>, créer une API REST avec Spring Boot, et le frontend avec <u>SvelteKit</u>. Le projet est au stade de modélisation de la base de données ; comprendre les relations entre les différentes entités est crucial pour définir une base de données viable et scalable. L'accent est surtout mis sur toute la conception du projet d'écrire du code. Il faut aussi écrire un <b>Contrat d'API avec Swagger</b> pour la clareté et la documentation. Crée des <u>User story</u> pour bien définir les features. <b><a href="https://i.postimg.cc/mr2CwDZf/Screenshot-7.png" target="_blank">Exemple de user story</a></b> <br/>  
  </p>
  
  <h3 id="breaking-header">Le projet NFT Solana</h3>
  <p>
    Celui-ci est un de mes projets de groupe les plus éprouvants. Nous avons tous vu la ruée vers l'or que représentaient les NFT en 2021. C'est pour cela que, avec deux amis axés sur le design graphique, nous avons tenté l'expérience de créer nos propres NFT Génératifs, à l'instar des CryptoPunks. J'étais le "chef de projet", sachant que j'étais le seul à développer le projet au niveau technique. Partant de zéro, nous avons créé une identité visuelle et trouvé le nom de <b>Pocket Hammies NFT</b>.Nous avons créé des parties distinctes en PNG avec différentes raretés pour qu'elles se superposent et créent un hamster avec une rareté X par le biais d'un script en JavaScript. <br>Ce projet personnel tombait pendant ma deuxième année, où je venais à peine de commencer à apprendre JavaScript. Alors, pour moi, créer un contrat sur la blockchain de Solana, c'était de la "rocket science". <br>Mais j'ai su trouver de l'aide auprès d'un jeune de Singapour que j'avais rencontré sur Discord. Nous avions des réunions à 3h du matin à cause du décalage horaire, et il m'a aidé à setup le lancement en passant par un template écrit en TypeScript. À cause des frais de blockchain, j'ai payé environ 600 CHF de ma poche pour le lancement. Le site fut hébergé sur Vercel. <br>

Aspect apprentissage : <br>

Même si l'aspect code est minime sur ce projet, je trouve pertinent de le citer car c'est tout ce qui entoure ce projet qui m'a vraiment apporté beaucoup. Il a fallu déterminer une direction, gérer les personnalités du projet et leurs avis, les deadlines, le stress que tout se passe bien lors du lancement à cause de l'argent investi. Créer de l'engouement sur les réseaux sociaux pour récolter un maximum "d'acheteurs" le jour du lancement. Gérer les possibles collaborations avec les autres NFT de la blockchain. <br>

Résultat : <br>

Nous avons réussi à créer une petite communauté autour du lancement sur Discord. Le jeune développeur qui nous aidait, ayant créé son NFT à côté avec des assets que nous lui avions vendus, grâce à un coup de poker, a lancé son projet avant le nôtre, amassant une somme avoisinant les 80'000$. La hype chez lui étant créée et les acheteurs ayant déjà investi chez lui n'avaient plus trop envie d'investir chez nous. Au final, nous avons vendu pour environ 3000$ de NFT et avons partagé la somme entre nous trois.<br>
    <b><a href="https://moonrank.app/collection/pocket_hammies" target="_blank">Voici un apercu de ce qui reste des NFT</a></b>
    <ImageContent src={team} />   
  </p>
  <h3 id="breaking-header">Les projet sur l'écologie et le changement climatique</h3>
  <p>
    Au cours de ma dernière année, j'ai axé mes projets sur le changement climatique, car cette problématique va s'intensifier dans les années à venir. Je trouvais pertinent de faire des recherches sur le sujet. Pour mon projet de spécialité, je me suis axé sur une analyse Data Science sur <b>La résilience d'un individu face aux changements climatiques</b>. Le déroulement de ce projet a d'abord commencé par une enquête sur Google Forms où je posais des questions aux élèves de mon université (SAE Institute). Les questions étaient faites pour effectuer une analyse ANOVA et définir un sentiment sur l'échelle de Likert. J'ai écrit cet <b><a href="https://medium.com/@florian.secretan/projet-de-sp%C3%A9cialisation-data-science-5c04d80c9dae" target="_blank"> article </a></b>sur Medium, où j'y décris les procédés plus en détails. <br>
    Mon mémoire de Bachelor est une recherche sur <b><a href="florian-display\src\assets\pdf\florian-secretan-memoire.pdf" download>Comment faciliter le monitoring individuel de sa consommation d'énergie
      dans le contexte de l'anthropocène?</a></b> Pendant l'écriture de mon bachelor j'ai pu être accompagné de <u>Nicolas Siorak, Economiste et Expert sur le climat</u>. Il a su me guider et me faire poser les bonnes questions lors du prototypage UI de mon application mobile. <br>
      Pour mes deux projets de dernière année j'ai eu la note de 5.4 / 6 (notation suisse) et la mention assez bien.
  </p>
  <ImageContent src={ecowise} />
  <h3 id="breaking-header">Mes autres projets.</h3>
  <p>Vous pouvez trouver tous mes autres projets sur GitHub, y compris depuis un simple jeu de poker en C++ sur la console, un forum à question en <u>PHP</u> et <u>MySQL</u> jusqu'à une petite application de messagerie web intégrant les prix des crypto-monnaies. Toutefois, ce qui compte vraiment pour moi n'est pas tant la pertinence de ces projets en eux-mêmes, mais plutôt l'expérience qu'ils m'ont apportée. Certes, le code est important, mais face au choix entre un petit projet ayant une utilité concrète et un projet plus générique, je privilégierais toujours le premier.
    <a id="githubimg" href="https://github.com/DigitalDanteCrypto" target="_blank"><img  src={github_logo} alt=""></a>
  </p>
  <h3 id="breaking-header">Mes références</h3>
  <div id="references">
    <ul>
      <li>Nicolas Paschoud</li>
      <li>Software Engineer, Data Engineer & DevOps</li>
      <li>nicolas.paschoud@gmail.com</li>
      <li>+41 79 882 30 90</li>
    </ul>
    <ul>
      <li>Nicolas Siorak</li>
      <li>Economiste, Expert Climatologue, Directeur Geneva Resilience Center</li>
      <li>+41 76 758 54 12</li>
    </ul>
  </div>

</div>

<style>
/* MOBILE */

@media screen and (min-width: 320px) {
#references {
  
}

.reusable-style-v1 {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 2rem;
  padding-right: 2rem;
}

#video-frame {
  display: none;
}

#myprojects {
  font-family: "Inter", sans-serif;
}

#breaking-header, h3 {
  color: rgba(38, 43, 56, 0.856);
  line-height: 2;
  font-weight: 600;
  margin: 10px 0;
}

p {
  color: rgb(55 65 81);
  font-weight: 400;
  line-height: 1.75rem;
}

a {
  text-decoration: none;
  color: inherit;
}

ul {
  margin: revert;
  padding: revert;
}

li {
  margin: 0.6rem;
}

video {
  max-width: 100%; /* Ensure video is not wider than the viewport */
  max-height: 100vh;
}

#githubimg {
  margin: 0 auto;
  padding-top: 20px;
}

#githubimg img {
  width: 30px;
  height: 30px;
}

/* DESKTOP */

@media screen and (min-width: 1024px){
  #references {
  display:flex;
}



}


}















/* DESKTOP */

@media screen and (min-width: 1024px){


  .reusable-style-v1 {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-left: 8rem;
    padding-right: 8rem;
    padding-bottom: 4rem;
    
}





    #video-frame {
        margin: 3rem;
    }
  #myprojects {
    font-family: "Inter", sans-serif;
  }

  #breaking-header {
    color: rgba(38, 43, 56, 0.856);
    line-height: 2;
    font-weight: 600;
    margin: 10px 0 10px 0;
  }

  p {
    --tw-text-opacity: 1;
    color: rgb(55 65 81 / var(--tw-text-opacity));
    font-weight: 400;
    line-height: 1.75rem;
  }
  h3 {
    color: rgba(38, 43, 56, 0.856);
    line-height: 2;
    font-weight: 600;
  }
  a {
    text-decoration: none;
    color: inherit
  }

  ul {
    margin: revert;
  padding: revert;
  }
  li {
    margin: 0.4rem;
  }
  video {
    max-width: 100%; /* Ensure video is not wider than the viewport */
    max-height: 100vh;
  }

  #githubimg {
    padding-top: 20px;
  }
  #githubimg img{
    width: 30px;
    height: 30px;
    
  }
}
</style>
