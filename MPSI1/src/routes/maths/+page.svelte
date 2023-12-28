<script>
  import "katex/dist/katex.min.css";
  import { onMount } from "svelte";

  let equation = "\\(1 + 1 = 1 \\implies \\text{« Je suis Napoléon »}\\)";
  let q = "\\( \\mathbb{Q} \\)";
  let r = "\\( \\mathbb{R} \\)";
  let cocu =
    "\\( cos(p) = \\frac{cosinq}{co}\\text{  donc  }cocu = \\frac{\\pi}{2} - q \\)";

  onMount(() => {
    document.addEventListener("DOMContentLoaded", () => {
      renderMathInElement(document.body, {
        delimiters: [
          { left: "\\(", right: "\\)", display: false },
          { left: "$$", right: "$$", display: true },
        ],
      });
    });
  });
</script>

<div
  class="h-full px-10 bg-base-200 py-20 flex flex-col items-center lg:items-start lg:px-20"
>
  <h1 class="text-3xl py-7">
    Mathématiques en classe préparatoire aux grandes écoles.
  </h1>
  <p>
    Voici un très sérieux résumé hebdomadaire des cours de mathathématiques
    enseignées par M. Molin.
  </p>
  <ul
    class="timeline timeline-vertical lg:timeline-horizontal bg-base-300 p-7 rounded-lg my-10"
  >
    <!-- 1 -->
    <li>
      <div class="timeline-start">25 septembre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_chocnap.showModal()"
      >
        Chocapics
      </div>
      <dialog id="my_modal_chocnap" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Chocapics</h3>
          <p class="py-4">
            Les personnes qui n'ont pas eu la chance de manger des Chocapics
            durant leur enfance, n'ont aucun avenir en mathématique. En effet,
            ce sont les labyrinthes derrière les boites de chocapics qui nous
            aprennent à partir du but afin de trouver le point de départ en
            remontant.
          </p>
          <h3 class="font-bold text-lg">Napoléon</h3>

          <div class="py-4">{@html equation}</div>

          <h3 class="font-bold text-lg">Citations de la semaine</h3>

          <p class="py-4">
            « Un grand bonhomme, Staline, il avait une de ces moustaches... »
            <br />
            « La vie c'est comme ce feutre, quand on est vieux et qu'on a plus de
            jus, on sert plus à rien »
            <br />
            « Ce cours est sponsorisé par Nestlé et CyberGhost VPN »
          </p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 2 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">2 octobre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_biq.showModal()"
      >
        Biquette
      </div>
      <dialog id="my_modal_biq" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Biquette</h3>
          <p class="py-4">
            Biquette, aka la Chèvre de M. Seguin doit être protégée du loup. On
            lui consitue donc un enclos, et une laisse d'une longueur qui oblige
            à Biquette de ne pas sortir de son enclos.
          </p>

          <h3 class="font-bold text-lg">Boulangerie</h3>

          <p class="py-4">
            Si la boulangerie est situé sur le trajet de l'école, je parcours
            moins de distance que si ma maison est située entre la boulangerie
            et l'école.
          </p>

          <h3 class="font-bold text-lg">Registre d'état civil</h3>

          <p class="py-4">
            Relations binaires : registre d'état civil, où tous les mariages
            sont tolérés. Que ça soit avec soi-même, ou même avec tous les gens
            du quartier.
          </p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 3 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">9 octobre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_isp.showModal()"
      >
        Ils sont partout
      </div>
      <dialog id="my_modal_isp" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Ils sont partout</h3>
          <p class="py-4">
            {@html q} est dense dans {@html r}, car entre n'importe quel couple
            de deux éléments de {@html q}, on trouve un élément de {@html r}
          </p>
          <h3 class="font-bold text-lg">Cocu</h3>

          <p class="py-4">{@html cocu}</p>
          <p>Je sais pas qui a compris ça, mais bon</p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 4 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">6 novembre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_phok.showModal()"
      >
        Cours applications
      </div>
      <dialog id="my_modal_phok" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <img
            src="https://cdn.discordapp.com/attachments/971357234980327424/1190030697868574740/broken-image-dark.png?ex=65a05174&is=658ddc74&hm=06a38ad1fec66cc836024f2f494fbc5ac4e626904d449100c26264aa1cb510d7&"
            alt="phoques"
            class="h-full w-full rounded-lg"
          />
          <p>Comprendra qui pourra</p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 5 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">20 novembre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_gend.showModal()"
      >
        Gendarmes
      </div>
      <dialog id="my_modal_gend" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Gendarmes</h3>
          <p class="pt-4">
            « Vous connaissez bien les gendarmes, vous, Sélim »
          </p>
          <p class="pb-4 text-end">– M. Molin</p>

          <h3 class="font-bold text-lg">Balançoire</h3>
          <p class="py-4">
            « Quand j'étais petit, j'était le meilleur en balançoire. J'étais
            tellement le meilleur que je faisais des tours autour de la barre. »
            <br />
            Contexte : raisonnance en physique
          </p>
          <h3 class="font-bold text-lg">Tours</h3>
          <p class="pt-4">« Détruisez-les, ces tours ! »</p>
          <p class="pb-4 text-end">– M. Vadée-le-Brun</p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 6 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">27 novembre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_ds.showModal()"
      >
        Prisonniers
      </div>
      <dialog id="my_modal_ds" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Prisonniers</h3>
          <p class="py-4">
            Contexte : suites fonctionnelles, points fixes et domaines stables. <br
            /> Chaque domaine stable est une prison, et selon la position du premier
            terme, il peut y avoir des transferts de prisoniers.
          </p>
          <h3 class="font-bold text-lg">Déterminisme social</h3>
          <p class="py-4">
            « Je suis convaincu que l'on peut échaper au déterminisme social :
            même si vos parents sont des délinquants, vous pourrez toujours
            travailler très dur en prépa et avoir la chance de pouvoir éspérer
            réussir votre vie »
          </p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 7 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">1er décembre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_nap.showModal()"
      >
        Napoléon
      </div>
      <dialog id="my_modal_nap" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Film Napoléon</h3>
          <p class="py-4">
            Rien de très spécial, une prosaïque sortie au cinéma avec M. Molin,
            à l'occasion de l'anniversaire des 219 ans de son couronnement.
          </p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 8 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">11 décembre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_napo.showModal()"
      >
        Napoléours
      </div>
      <dialog id="my_modal_napo" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Napoléours</h3>
          <p class="py-4">
            Le divin avènement de Napoléours 1er, notre Empereur à tous.
          </p>
          <img
            src="https://cdn.discordapp.com/attachments/971357234980327424/1189561209654083604/Sans_titre.jpg?ex=659e9c35&is=658c2735&hm=4637e16d0a1a308d93ebf430e8bd209c4097fc2bd31df49073cebd830791bb81&"
            alt="Napléours"
            class="max-h-32 w-auto mx-auto rounded-md lg:max-h-48 mb-4"
          />

          <h3 class="font-bold text-lg">Suite stationnaire</h3>
          <p class="py-3">L'image se suffit à elle-même.</p>
          <img
            src="https://media.discordapp.net/attachments/971357234980327424/1190043414281076818/image.png?ex=65a05d4b&is=658de84b&hm=a201d254538a20850204e5d13f147fd5f115ae5e7ed592913ca2ca5c69e2796e&=&format=webp&quality=lossless"
            alt=""
            class="max-h-32 w-auto mx-auto rounded-md lg:max-h-48"
          />

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>

    <!-- 9 -->

    <li>
      <hr class="bg-primary" />
      <div class="timeline-start">18 décembre</div>
      <div class="timeline-middle">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 20 20"
          fill="currentColor"
          class="w-5 h-5"
          ><path
            fill-rule="evenodd"
            d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.857-9.809a.75.75 0 00-1.214-.882l-3.483 4.79-1.88-1.88a.75.75 0 10-1.06 1.061l2.5 2.5a.75.75 0 001.137-.089l4-5.5z"
            clip-rule="evenodd"
          /></svg
        >
      </div>
      <div
        class="timeline-end btn timeline-box"
        onclick="my_modal_cit.showModal()"
      >
        Vacances
      </div>
      <dialog id="my_modal_cit" class="modal modal-bottom sm:modal-middle">
        <div class="modal-box">
          <h3 class="font-bold text-lg">Citation de la semaine</h3>
          <p class="py-4">
            « Une promo de perdue, 10 de retrouvées, c'est ce que l'on se dit
            entre profs de prépa. »
          </p>

          <div class="modal-action">
            <form method="dialog">
              <!-- if there is a button in form, it will close the modal -->
              <button class="btn">Fermer</button>
            </form>
          </div>
        </div>
      </dialog>

      <hr class="bg-primary" />
    </li>
  </ul>
</div>
