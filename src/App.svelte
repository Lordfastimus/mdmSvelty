<script>
  import Nav from "./comp/Nav.svelte";
  import Footer from "./comp/Footer.svelte";
  import Sections from "./comp/Sections/Sections.svelte";
</script>

<style lang="scss">
  :global(:root) {
    --dark-color: #1e1e1e;
    --dark-color-light: #2b2b2b;
    --main-color: #ff3566;
    --main-color-red: 255;
    --main-color-green: 53;
    --main-color-blue: 102;
    --light-color: #fff;
    --font-size: 16px;
    --light-font-color: #fff;
    font-size: var(--font-size);
    --font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
    font-family: var(--font-family);
    section {
      padding-top: 10vh;
      padding-bottom: 10vh;
    }
    h1 {
      font-size: 2em;
      font-weight: 700;
    }

    @media (min-width: 480px) {
      h1 {
        font-size: 3em;
      }
    }
  }
  .container {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
</style>

<div class="container">
  <Nav />
  <Sections />
  <Footer />
</div>
