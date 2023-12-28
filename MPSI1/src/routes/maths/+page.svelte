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

<div class="h-svh bg-base-200 p-20">
  <ul class="timeline timeline-vertical lg:timeline-horizontal">
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

      <hr />
    </li>

    <!-- 2 -->

    <li>
      <hr />
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

      <hr />
    </li>

    <!-- 3 -->

    <li>
      <hr />
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

      <hr />
    </li>

    <!-- 4 -->

    <li>
      <hr />
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

      <hr />
    </li>

    <!-- 5 -->

    <li>
      <hr />
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

      <hr />
    </li>

    <!-- 6 -->

    <li>
      <hr />
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

      <hr />
    </li>

    <!-- 7 -->

    <li>
      <hr />
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

      <hr />
    </li>
  </ul>
</div>
