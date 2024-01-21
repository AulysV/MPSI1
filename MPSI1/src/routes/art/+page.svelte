<h1 class="text-3xl text-center font-semibold py-10 lg:text-5xl">
  L'art du 21e siècle
</h1>

<!-- <script>
  let images = [
    "https://media.discordapp.net/attachments/971357234980327424/1192211569841541180/htry.jpeg?ex=65a8408c&is=6595cb8c&hm=4a343a4798d1870d149d94f521b767eac79bc50cb32f4028eb2c824220de0700&=&format=webp",
    "https://media.discordapp.net/attachments/971357234980327424/1192211570101596211/drg.jpeg?ex=65a8408c&is=6595cb8c&hm=a8b3ec37d2ead526422e73015e58a55ea8722087dafd4d5fac07a2f3f6b0f2f1&=&format=webp",
    "https://media.discordapp.net/attachments/971357234980327424/1192211570420367470/qzdqzdqzd.jpeg?ex=65a8408c&is=6595cb8c&hm=5d9a56aa16b10fa3a50f044a16ad88b5c677d936eb59800dc5279de02250ead5&=&format=webp",
    "https://media.discordapp.net/attachments/971357234980327424/1192211570810433656/qdzqz.jpeg?ex=65a8408c&is=6595cb8c&hm=f4ae717a31f7a78098da3b130b42456fdf1441748ed462d48c6b9018a7cd9075&=&format=webp",
    "https://media.discordapp.net/attachments/971357234980327424/1192211571091456082/Sans_titre.jpg?ex=65a8408c&is=6595cb8c&hm=f13d3cfe3e63af677ce8af2e503f21d1707a81081af1f95c224a3155b3eb03b6&=&format=webp",
    // Ajoutez autant d'images que vous le souhaitez
  ];

  let currentImage = images[0];

  function changeImage(index) {
    currentImage = images[index];
  }
</script>

<div id="gallery">
  {#each images as image, index (image)}
    <img
      src={image}
      alt="Thumbnail"
      class:thumbnail={currentImage === image}
      on:click={() => changeImage(index)}
    />
  {/each}
</div>

<style>
  #gallery {
    margin: 3em;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 1em;
    justify-content: center;
    padding: 1em;
  }

  .thumbnail {
    width: 100%;
    height: auto;
    border-radius: 10px;
    cursor: pointer;
    transition: transform 0.3s ease;
  }

  .thumbnail:hover {
    transform: scale(1.05);
  }
</style> -->

<!-- <div class="h-full w-100 my-20">
  <img
    src="https://media.discordapp.net/attachments/971357234980327424/1192211569841541180/htry.jpeg?ex=65a8408c&is=6595cb8c&hm=4a343a4798d1870d149d94f521b767eac79bc50cb32f4028eb2c824220de0700&=&format=webp"
    class="rounded-box ml-auto mr-auto"
  />
</div> -->

<div id="gallery">
  <div class="photoss">
    <img
      src="https://media.discordapp.net/attachments/971357234980327424/1192211569841541180/htry.jpeg?ex=65a8408c&is=6595cb8c&hm=4a343a4798d1870d149d94f521b767eac79bc50cb32f4028eb2c824220de0700&=&format=webp"
      alt="Photo 1"
    />
  </div>
  <div class="photoss">
    <img
      src="https://media.discordapp.net/attachments/971357234980327424/1192211570101596211/drg.jpeg?ex=65a8408c&is=6595cb8c&hm=a8b3ec37d2ead526422e73015e58a55ea8722087dafd4d5fac07a2f3f6b0f2f1&=&format=webp"
      alt="Photo 2"
    />
  </div>
  <div class="photoss">
    <img
      src="https://media.discordapp.net/attachments/971357234980327424/1192211570420367470/qzdqzdqzd.jpeg?ex=65a8408c&is=6595cb8c&hm=5d9a56aa16b10fa3a50f044a16ad88b5c677d936eb59800dc5279de02250ead5&=&format=webp"
      alt="Photo 3"
    />
  </div>
  <div class="photoss">
    <img
      src="https://media.discordapp.net/attachments/971357234980327424/1192211570810433656/qdzqz.jpeg?ex=65a8408c&is=6595cb8c&hm=f4ae717a31f7a78098da3b130b42456fdf1441748ed462d48c6b9018a7cd9075&=&format=webp"
      alt="Photo 4"
    />
  </div>
  <div class="photoss">
    <img
      src="https://media.discordapp.net/attachments/971357234980327424/1192211571091456082/Sans_titre.jpg?ex=65a8408c&is=6595cb8c&hm=f13d3cfe3e63af677ce8af2e503f21d1707a81081af1f95c224a3155b3eb03b6&=&format=webp"
      alt="Photo 5"
    />
  </div>
  <!-- Ajoutez plus d'images si nécessaire -->
</div>

<style>
  #gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
    padding: 15px;
  }

  .photoss {
    overflow: hidden;
    border-radius: 15px;
  }

  .photoss img {
    width: 100%;
    height: auto;
    border-radius: 15px;
  }
</style>
