<!-- Hero -->

<script>
  import { gsap } from "gsap";
  let rotation = 0;

  const rotateImage = () => {
    rotation += 360; // Augmente la rotation de 360 degrés à chaque clic
    gsap.to("#img", {
      rotation,
      duration: 1,
      ease: "power2.inOut",
    });
  };

  import nap from "$lib/img/nap.jpg";
</script>

<div class="hero h-svh bg-base-200">
  <div class="hero-content flex-col lg:flex-row max-w-4xl">
    <img
      src={nap}
      class="max-w-52 mx-10 rounded-full"
      id="img"
      on:click={rotateImage}
    />

    <div>
      <h1 class="text-5xl font-bold">Bonjour</h1>
      <p class="py-6">
        Vous êtes actuellement sur l'incroyable et merveilleux site internet de
        la MPSI1.
      </p>
    </div>
  </div>
</div>
