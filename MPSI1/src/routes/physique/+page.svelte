<script>
  import "katex/dist/katex.min.css";
  import { onMount } from "svelte";

  let r = "\\( \\mathbb{R} \\)";

  onMount(() => {
    renderMathInElement(document.body, {
      delimiters: [
        { left: "\\(", right: "\\)", display: false },
        { left: "$$", right: "$$", display: true },
      ],
    });
  });

  import hehe from "$lib/hehe.mp4";
</script>

<div class="h-full px-10 bg-base-200 pb-10 lg:items-start lg:px-20">
  <h1 class="text-3xl text-center font-semibold py-10 lg:text-5xl">
    Physique.
  </h1>
  <div id="image" class="rounded-lg h-64">
    <div id="blur" class="rounded-lg"></div>
  </div>
  <p class="py-3 text-xl lg:text-3xl mb-5">
    Soyons polis, ne parlons pas de chimie.
  </p>

  <!-- Content -->

  <div class="collapse collapse-arrow bg-base-300 mb-3">
    <input type="radio" name="my-accordion-2" checked="checked" />
    <div class="collapse-title text-xl font-medium">Citations :</div>
    <div class="collapse-content">
      <div class="chat chat-start">
        <div class="chat-footer">
          <!-- M. Vadée-le-Brun -->
          <time class="text-xs opacity-50">Assez souvent</time>
        </div>
        <div class="chat-bubble">
          Au pire j'ai perdu 1 point mais j'ai gagné 30 secondes 🤷
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Elec
          <time class="text-xs opacity-50">Automne</time>
        </div>
        <div class="chat-bubble">
          Le disjoncteur peut pas savoir que c'est Bob qui vient de se connecter
          au réseau EDF
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Filtres
          <time class="text-xs opacity-50">Automne</time>
        </div>
        <div class="chat-bubble">Détruisez-les, ces tours !</div>
      </div>

      <!-- <div class="chat chat-start">
        <div class="chat-footer">
          Chimie
          <time class="text-xs opacity-50">Automne</time>
        </div>
        <div class="chat-bubble"></div>
      </div> -->

      <div class="chat chat-start">
        <div class="chat-footer">
          DM 5
          <time class="text-xs opacity-50">Novembre</time>
        </div>
        <div class="chat-bubble">
          Les Bobs sont un peu déçus de constater qu’on ne peut vraiment pas
          mourir à beaucoup ensemble dans ce fichu pays.
          <br /> <br />
          Grâce à cette méthode développée par notre cher camarade, on peut tuer
          les Bob par paquets de 45 ! C'est plutôt efficace. <br />
          Ce camarade ne serait pas d'origine Allemande ?
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Méca
          <time class="text-xs opacity-50">Décembre</time>
        </div>
        <div class="chat-bubble">
          Reprenons le cas où je saute par la fenêtre.
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Chimie (💀)
          <time class="text-xs opacity-50">Janvier</time>
        </div>
        <div class="chat-bubble">
          Donnez vos enzymes SVP <br /> L'antilope sait que son prédateur peut pas
          courir longtemps. Mais nous, on peut harceler l'antilope en faisant notre
          petit footing jusqu'à ce qu'elle tombe de chaud !
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Méca
          <time class="text-xs opacity-50">Janvier</time>
        </div>
        <div class="chat-bubble">
          Alice et Bob ont une idée en tête : Pousser Alice suffisamment fort
          pour qu’elle puisse faire un tour complet.
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Force centrale
          <time class="text-xs opacity-50">Janvier</time>
        </div>
        <div class="chat-bubble">
          L'ISS c'est juste un petit centre d'entrainement pour les bébés
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Champs
          <time class="text-xs opacity-50">Janvier</time>
        </div>
        <div class="chat-bubble">
          Je me branche au nuage et je lui prends toute son électricité
        </div>
      </div>

      <div class="chat chat-start">
        <div class="chat-footer">
          Champs
          <time class="text-xs opacity-50">Janvier</time>
        </div>
        <div class="chat-bubble">
          Par récurrence rapide sur {@html r}
        </div>
      </div>
    </div>
  </div>
  <div class="collapse collapse-arrow bg-base-300 mb-3">
    <input type="radio" name="my-accordion-2" />
    <div class="collapse-title text-xl font-medium">
      « Pour ralentir une réaction, il suffit de ralentir la réaction »
    </div>
    <div class="collapse-content">
      <video controls width="500">
        <source src={hehe} type="video/mp4" />
        <!-- Ajoutez d'autres sources pour la compatibilité avec différents navigateurs -->
        Votre navigateur ne supporte pas la balise video.
      </video>
      <p class="pt-4">Par Benjamin</p>
    </div>
  </div>
</div>

<style>
  #image {
    background-image: url("$lib/img/6.jpg");
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
    margin-bottom: 2em;
  }
  #blur {
    /* backdrop-filter: blur(7px); */
    background: rgba(0, 0, 0, 0);
    height: 100%;
    width: auto;
  }

  video {
    border-radius: 12px;
  }
</style>
