<script></script>

<footer>
  <div id="footer-content">
    <span> Merci pour votre lecture </span>

    <hr id="line-bidule" />
    <p class="disclaimer">Disclaimer :</p>
    <p class="disclaimer">
      This page was made by florian, in a dopamine rush mixed with stress and
      caffeine, no intend to steal any design, it was made for Atipik career
      purpose ❤️
    </p>
    <p  class="disclaimer">It was made with Svelte</p>
  </div>
  <div class="contact-info">
    <div class="item">Chemin des Vignes, 31. 1213 Petit-Lancy</div>
    <div class="item">
      <a href="mailto:florian.secretan@gmail.com">florian.secretan@gmail.com</a>
    </div>
    <div class="item">
      <a href="tel:+1234567890">+41 79 933 89 42</a>
    </div>
  </div>
</footer>

<style>
  /* MOBILE */

  @media screen and (min-width: 320px) {
    footer {
      font-family: "Inter", sans-serif;
      font-weight: 600;
      font-size: 1.75rem;
      background: linear-gradient(135deg, #0e1116 33.33%, #1c2027);
    }
    span {
      color: white;
    }
    #footer-content {
      margin-left: auto;
      margin-right: auto;
      padding-left: 1.5rem;
      padding-right: 1.5rem;
      padding-top: 2rem;
    }

    #line-bidule {
      margin-bottom: 2rem;
      margin-top: 2rem;
      border-top-width: 1px;
      color: inherit;
      height: 0;
      --tw-border-opacity: 1;
      border-color: rgb(55 65 81 / var(--tw-border-opacity));
    }

    .disclaimer {
      text-align: center;
      font-size: 0.6rem;
      color: white;
    }

    .contact-info {
      font-size: small;
      padding: 1rem;
      text-align: center;
    }

    .item {
      display: flex;
      flex-direction: column;
      align-items: center;
      color: #ed6a0c;
      margin: 1rem;
    }

    .item a {
      color: #ed6a0c;
      text-decoration: none;
    }

    .item a:hover {
      text-decoration: underline;
    }
  }

  /* DESKTOP */

  @media screen and (min-width: 1024px) {
    footer {
      font-family: "Inter", sans-serif;
      font-weight: 600;
      font-size: 1.75rem;
      background: linear-gradient(135deg, #0e1116 33.33%, #1c2027);
    }
    span {
      color: white;
    }
    #footer-content {
      margin-left: auto;
      margin-right: auto;
      padding-left: 1.5rem;
      padding-right: 1.5rem;
      padding-top: 2rem;
    }

    #line-bidule {
      margin-bottom: 2rem;
      margin-top: 2rem;
      border-top-width: 1px;
      color: inherit;
      height: 0;
      --tw-border-opacity: 1;
      border-color: rgb(55 65 81 / var(--tw-border-opacity));
    }

    .disclaimer {
      text-align: center;
      font-size: 0.6rem;
      color: white;
    }

    .contact-info {
      font-size: small;
      padding: 1rem;
      display: flex;
      justify-content: center;
    }

    .item {
      display: flex;
      flex-direction: column;
      align-items: center;
      color: #ed6a0c;
      margin: 1rem;
    }

    .item a {
      color: #ed6a0c;
      text-decoration: none;
    }

    .item a:hover {
      text-decoration: underline;
    }
  }
</style>
