<script>
</script>

<svelte:head>
  <link
    href="https://fonts.googleapis.com/css?family=Press Start 2P"
    rel="stylesheet"
  />
</svelte:head>

<div class="hero" style="font-size: 2rem;">
  <div class="typo">
    <img src="/assets/azilic.webp" height="100%" alt="MERAZ" />
  </div>
</div>

<style lang="scss">
  .hero {
    position: relative;
    width: 100%;
    height: 100vh;
    background-image: url("/assets/Frame (1).webp");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat; // Prevents repeating
    text-align: center;
    scroll-snap-align: start;

    @media (max-width: 900px) {
      background-size: contain;
      background-position: top;
    }
  }
  .typo {
    position: absolute;
    height: 65vh;
    width: 100vw;
    top: 69%;
    left: 50%;
    transform: translate(-50%, -50%);
    img {
      height: 100%;
      width: 80%;
      object-fit: contain;
    }
    @media (max-width: 1000px) {
      top: 65%;
    }
    @media (max-width: 900px) {
      top: 53%;
    }
    @media (max-width: 860px) {
      top: 37%;
    }
    @media (max-width: 650px) {
      top: 33%;
    }
    @media (max-width: 530px) {
      top: 27%;
    }
    @media (max-width: 430px) {
      top: 20%;
    }
  }
</style>
