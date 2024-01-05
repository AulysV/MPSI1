<script>
  let motdepasseentré = "";
  const vraimotdepasse = "monkey";

  function verif() {
    if (motdepasseentré === vraimotdepasse) {
      const messageDiv = document.getElementById("message");
      messageDiv.textContent =
        "Voici une petite musique en attendant les 500000 Francs CFA";

      setTimeout(() => {
        window.open("https://www.youtube.com/watch?v=dQw4w9WgXcQ", "_blank");
      }, 5000);
    } else {
      const messageDiv = document.getElementById("message");
      messageDiv.textContent = "Mot de passe incorrect.";
    }
  }
</script>

<div class="h-svh text-center flex flex-col justify-center items-center p-10">
  <h1 class="text-3xl text-center font-semibold my-5">
    Veuillez entrer le mot de passe :
  </h1>

  <input
    type="text"
    class="input input-bordered w-full max-w-xs my-5"
    bind:value={motdepasseentré}
    placeholder="Mot de passe"
  />
  <button class="btn btn-sm sm:btn-sm md:btn-md my-5" on:click={verif}
    >Vérifier</button
  >

  <div id="message"></div>
</div>
