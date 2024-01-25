<script>
  import "../app.css";
  // import { gsap } from "gsap";

  // onMount(() => {
  //   const rotateButton = () => {
  //     gsap.to("#initial-button", {
  //       rotation: "+=360",
  //       duration: 1,
  //       ease: "power2.inOut",
  //     });
  //   };
  //   rotateButton();
  // });
</script>

<!-- Navbar -->

<div class="navbar bg-base-300">
  <label class="swap swap-flip text-9xl">
    <!-- this hidden checkbox controls the state -->
    <input type="checkbox" />
    <img
      src="https://cdn.discordapp.com/attachments/971357234980327424/1189545367570759711/logoMpsi1.png?ex=659e8d74&is=658c1874&hm=c4b9c041a7a17e320387ee3dd1bb2281d3c36bfa0a642b8e4eb9691930e62ffc&"
      class="max-w-10 mx-2 swap-off"
    />
    <img
      src="https://cdn.discordapp.com/attachments/971357234980327424/1189551882537017414/logoMpsi12.png?ex=659e9385&is=658c1e85&hm=eaf6029230099c280c30fddacdc6fd89233aed4906dde81249cd2964d7235320&"
      class="max-w-10 mx-2 swap-on"
    />
  </label>

  <div class="navbar-start">
    <div class="dropdown">
      <div tabindex="0" role="button" class="btn btn-ghost lg:hidden">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h8m-8 6h16"
          />
        </svg>
      </div>
      <ul
        tabindex="0"
        class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52"
      >
        <li><a href="/napo">Napoléours</a></li>
        <!-- <li>
          <a>Matières</a>
          <ul class="p-2">
            <li><a href="/maths">Maths</a></li>
            <li><a>Submenu 2</a></li>
          </ul>
        </li> -->

        <!-- <li>
          <a href="https://www.instagram.com/ord_kevin7256/" target="_blank"
            >Échec</a
          >
        </li> -->

        <li><a href="/maths">Maths</a></li>
        <!-- <li><a href="/art">Art</a></li> -->
        <li>
          <a href="/physique">Physique</a>
        </li>
        <li><a href="/autres">Autres</a></li>
      </ul>
    </div>
    <a class="btn btn-ghost text-xl" href="/">Accueil</a>
  </div>

  <div class="navbar-center hidden lg:flex">
    <ul class="menu menu-horizontal px-1">
      <li><a href="/napo">Napoléours</a></li>
      <!-- <li>
        <details>
          <summary>Matières</summary>
          <ul class="p-2">
            <li><a href="/maths">Maths</a></li>
            <li><a>Submenu 2</a></li>
          </ul>
        </details>
      </li> -->

      <!-- <li>
        <a href="https://www.instagram.com/ord_kevin7256/" target="_blank"
          >Échec</a
        >
      </li> -->

      <li><a href="/maths">Maths</a></li>
      <!-- <li><a href="/art">Art</a></li> -->
      <li>
        <a href="/physique">Physique</a>
      </li>
      <div class="indicator">
        <span class="indicator-item badge badge-primary text-xs">New</span>
      </div>

      <li>
        <a href="/autres">Autres</a>
      <!-- </li>
      <div class="indicator">
        <span class="indicator-item badge badge-primary text-xs">New</span>
      </div> -->
    </ul>
  </div>

  <div class="navbar-end mx-4">
    <a
      href="https://www.instagram.com/napoleon_mpsi1/?utm_source=ig_web_button_share_sheet&igshid=OGQ5ZDc2ODk2ZA=="
      target="_blank"><i class="fa-brands fa-instagram text-3xl"></i></a
    >
  </div>
</div>

<slot />

<!-- Footer -->

<!-- <footer class="footer p-7 bg-neutral text-neutral-content">
  <aside>
    <img
      src="https://cdn.discordapp.com/attachments/971357234980327424/1189545367344251021/aulys.png?ex=659e8d74&is=658c1874&hm=9f7e9b724462d92e96dd6d0581b623ecc2995c40799d725d680ed49a3c00c9c8&"
      class="max-w-14"
    />
    <p class="max-w-20">Coucou cé mwa Aulys la tutel</p>
  </aside>
  <nav>
    <header class="footer-title">Rézo socio</header>
    <div class="grid grid-flow-col gap-4">
      <a href="https://discord.gg/D8mpMaA8mj" target="_blank"
        ><i class="fa-brands fa-discord text-xl"></i></a
      >
      <a
        href="https://www.instagram.com/napoleon_mpsi1/?utm_source=ig_web_button_share_sheet&igshid=OGQ5ZDc2ODk2ZA=="
        target="_blank"><i class="fa-brands fa-instagram text-xl"></i></a
      >
    </div>
  </nav>
</footer> -->

<footer class="footer footer-center p-10 bg-base-300 text-base-content rounded">
  <nav class="grid grid-flow-col gap-4">
    <button onclick="my_modal_ap.showModal()">À propos</button>
    <dialog id="my_modal_ap" class="modal modal-bottom sm:modal-middle">
      <div class="modal-box text-left">
        <h3 class="font-bold text-lg">Par qui ?</h3>
        <p class="py-4">
          <a
            href="https://github.com/AulysV"
            target="_blank"
            rel="noopener noreferrer"
            class="link-hover">Une certaine personne du nom de Aulys</a
          >
        </p>
        <h3 class="font-bold text-lg">Avec quoi ?</h3>
        <p class="py-4">
          Svelte (framework JS) + TailwindCSS (composants : daisyUI)
        </p>
        <h3 class="font-bold text-lg">Pourquoi ?</h3>
        <p class="py-4">
          Parce que c'est réconfortant, en prépa, de se dire qu'on peut avoir
          quelque fois (mais rarement) du temps à perdre.
        </p>
        <div class="modal-action">
          <form method="dialog">
            <!-- if there is a button in form, it will close the modal -->
            <button class="btn">Fermer</button>
          </form>
        </div>
      </div>
    </dialog>

    <button onclick="my_modal_cont.showModal()">Contact</button>
    <dialog id="my_modal_cont" class="modal modal-bottom sm:modal-middle">
      <div class="modal-box text-left">
        <h3 class="font-bold text-lg">Contact</h3>
        <p class="pt-4">
          Si faute <span class="line-through">d'orthogrpahe</span> de frappe, suggestion,
          déclaration de guerre des PCSI2 :
        </p>
        <ul class="mt-3">
          <li>
            <a
              href="https://discord.com/users/637695900382134303"
              target="_blank"
              rel="noopener noreferrer"
              class="link-primary">Discord</a
            >
          </li>
        </ul>

        <div class="modal-action">
          <form method="dialog">
            <!-- if there is a button in form, it will close the modal -->
            <button class="btn">Fermer</button>
          </form>
        </div>
      </div>
    </dialog>
  </nav>
  <aside>
    <p>Copyright © 2024 – All rights reserved by nobody</p>
  </aside>
</footer>

<!-- Toast -->

<!-- <div class="toast">
  <div
    class="bg-base-300 h-15 w-15 flex items-center justify-center rounded-full p-3"
  >
    <label class="swap swap-rotate">
      <input type="checkbox" class="theme-controller" value="sunset" />

      <svg
        class="swap-on fill-current w-10 h-10"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        ><path
          d="M5.64,17l-.71.71a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l.71-.71A1,1,0,0,0,5.64,17ZM5,12a1,1,0,0,0-1-1H3a1,1,0,0,0,0,2H4A1,1,0,0,0,5,12Zm7-7a1,1,0,0,0,1-1V3a1,1,0,0,0-2,0V4A1,1,0,0,0,12,5ZM5.64,7.05a1,1,0,0,0,.7.29,1,1,0,0,0,.71-.29,1,1,0,0,0,0-1.41l-.71-.71A1,1,0,0,0,4.93,6.34Zm12,.29a1,1,0,0,0,.7-.29l.71-.71a1,1,0,1,0-1.41-1.41L17,5.64a1,1,0,0,0,0,1.41A1,1,0,0,0,17.66,7.34ZM21,11H20a1,1,0,0,0,0,2h1a1,1,0,0,0,0-2Zm-9,8a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V20A1,1,0,0,0,12,19ZM18.36,17A1,1,0,0,0,17,18.36l.71.71a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41ZM12,6.5A5.5,5.5,0,1,0,17.5,12,5.51,5.51,0,0,0,12,6.5Zm0,9A3.5,3.5,0,1,1,15.5,12,3.5,3.5,0,0,1,12,15.5Z"
        /></svg
      >

      <svg
        class="swap-off fill-current w-10 h-10"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        ><path
          d="M21.64,13a1,1,0,0,0-1.05-.14,8.05,8.05,0,0,1-3.37.73A8.15,8.15,0,0,1,9.08,5.49a8.59,8.59,0,0,1,.25-2A1,1,0,0,0,8,2.36,10.14,10.14,0,1,0,22,14.05,1,1,0,0,0,21.64,13Zm-9.5,6.69A8.14,8.14,0,0,1,7.08,5.22v.27A10.15,10.15,0,0,0,17.22,15.63a9.79,9.79,0,0,0,2.1-.22A8.11,8.11,0,0,1,12.14,19.73Z"
        /></svg
      >
    </label>
  </div>
</div> -->

<div class="toast toast-end">
  <div class="dropdown dropdown-left dropdown-end mx-4">
    <div
      tabindex="0"
      role="button"
      class="btn m-1 bg-neutral text-neutral-content"
    >
      Thème
      <svg
        width="12px"
        height="12px"
        class="h-2 w-2 fill-current opacity-60 inline-block"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 2048 2048"
        ><path d="M1799 349l242 241-1017 1017L7 590l242-241 775 775 775-775z"
        ></path></svg
      >
    </div>
    <ul
      tabindex="0"
      class="dropdown-content z-[1] p-3 shadow-2xl bg-base-300 rounded-box w-52 px-30"
    >
      <li>
        <input
          type="radio"
          name="theme-dropdown"
          class="theme-controller btn btn-sm btn-block btn-ghost justify-start"
          aria-label="Par défaut"
          value="sunset"
        />
      </li>
      <li>
        <input
          type="radio"
          name="theme-dropdown"
          class="theme-controller btn btn-sm btn-block btn-ghost justify-start"
          aria-label="Café"
          value="coffee"
        />
      </li>
      <li>
        <input
          type="radio"
          name="theme-dropdown"
          class="theme-controller btn btn-sm btn-block btn-ghost justify-start"
          aria-label="Cyberpunk"
          value="cyberpunk"
        />
      </li>
      <li>
        <input
          type="radio"
          name="theme-dropdown"
          class="theme-controller btn btn-sm btn-block btn-ghost justify-start"
          aria-label="Nord"
          value="nord"
        />
      </li>
      <li>
        <input
          type="radio"
          name="theme-dropdown"
          class="theme-controller btn btn-sm btn-block btn-ghost justify-start"
          aria-label="Night"
          value="night"
        />
      </li>
    </ul>
  </div>
</div>
