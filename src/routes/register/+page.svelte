<script>
  import { sidebarOpen } from "./../../lib/stores.js";
  import SectionHeader from "$lib/components/SectionHeader.svelte";
  $: $sidebarOpen = false;
</script>

<svelte:head>
  <title>Register | Meraz '24</title>
  <script
    type="text/javascript"
    src="https://unpkg.com/vis-timeline@latest/standalone/umd/vis-timeline-graph2d.min.js"
  ></script>
  <link
    href="https://unpkg.com/vis-timeline@latest/styles/vis-timeline-graph2d.min.css"
    rel="stylesheet"
    type="text/css"
  />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@400;700;900&family=Cormorant+Upright:wght@300;400;500;600;700&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<div class="container">
  <div class="heading">
    <SectionHeader name="Registration" />
  </div>
  <div class="box">
    <a
      href="https://docs.google.com/forms/d/e/1FAIpQLSd2NIYm9WLTy6KWUkkEOu10dI7ci8LDubXjhF4MyIubNsKIvg/viewform?usp=sharing"
      class="redirect-button"
      target="_blank"
      rel="noopener noreferrer"
    >
      Fest Pass
    </a>
    <a
      href="https://docs.google.com/forms/d/e/1FAIpQLSfwyK-BXZXdWJWk8vFn3QdRcoI_C64NO9eMX_9LQR1ZG-WHnA/viewform?usp=sf_link"
      class="redirect-button"
      target="_blank"
      rel="noopener noreferrer"
    >
      One Day Pass
    </a>
  </div>
</div>

<style>
  .container {
    background-image: url("/assets/schedule_bg.jpeg");
    font-family: LibreBaskerville;
    font-size: 1.5rem;
    align-items: center;
    background-size: cover;
    padding-bottom: 9.563rem;
    background-position: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    height: 100vh;
  }

  .heading {
    position: relative;
    margin-bottom: 20vh;
  }

  .box {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 2rem; /* Space between buttons */
  }

  .redirect-button {
    padding: 10px 40px;
    border-radius: 10px;
    border: 2px solid #bfbfbf;
    text-align: center;
    font-family: LibreBaskerville;
    transition:
      background-color 0.3s ease,
      font-weight 0.3s ease,
      color 0.3s ease;
  }

  .redirect-button:hover {
    background-color: #add8e6; /* Light blue color */
    font-weight: 900;
    color: #121212;
  }
</style>
