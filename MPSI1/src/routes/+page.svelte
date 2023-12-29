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
</script>

<div class="hero h-svh bg-base-200">
  <div class="hero-content flex-col lg:flex-row max-w-4xl">
    <img
      src="https://cdn.discordapp.com/attachments/971357234980327424/1189545367876948048/nap.jpg?ex=659e8d74&is=658c1874&hm=719f55e051ab64608491510b0e5d623fcae787238d3debb366541a5b59ccba22&"
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
