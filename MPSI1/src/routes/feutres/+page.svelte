<script>
  import feutre1 from "$lib/img/feutre1.png";
  import feutre2 from "$lib/img/feutre2.png";
  import feutre3 from "$lib/img/feutre3.png";
</script>

<div class="hero min-h-screen" id="hero">
  <div class="hero-overlay bg-opacity-40"></div>
  <div class="hero-content text-center text-neutral-content">
    <div class="max-w-none">
      <h1 class="text-6xl mb-14 lg:text-8xl font-bold">
        Le feutre de Napoléon
      </h1>
      <p class="mb-14 text-2xl font-bold lg:text-3xl">
        Découvrez les feutres ultimes, utilisés par l'Empereur lui-même.
      </p>
    </div>
  </div>
</div>
<!-- <h1 class="text-3xl font-semibold py-10 lg:text-5xl">
    Achetez les feutres ultimes
  </h1> -->

<img src={feutre1} alt="Feutre 1" class="my-15" />
<img src={feutre2} alt="Feutre 2" class="my-15" />
<img src={feutre3} alt="Feutre 3" class="my-15" />

<div class="hero min-h-screen" id="hero2">
  <div class="hero-overlay bg-opacity-40"></div>
  <div class="hero-content text-neutral-content">
    <div class="max-w-none">
      <h1 class="text-6xl mb-14 lg:text-8xl font-bold">Convaincus ?</h1>
      <p class="mb-2 text-2xl font-bold lg:text-3xl">
        Achetez cet artéfact historique dès maintenant !
      </p>
      <p class="mb-14 text-md font-bold">
        Disponible pour seulement 99.98€ (HT) la pièce
      </p>
      <a href="http://www.youtube.com/watch?v=o-YBDTqX_ZU"
        ><button class="btn btn-primary">Acheter</button></a
      >
    </div>
  </div>
</div>

<style>
  #hero {
    background-image: url("$lib/img/bg.jpg");
  }
  #hero2 {
    background-image: url("$lib/img/bg2.jpg");
  }
</style>
