<script>
import Container1200 from "$lib/container-1200.svelte";
</script>

<header>
  <Container1200>
    <div class="header-items">
      <div class="logo">
        <a href="/"><img src="images/logos/logo.svg" alt="davejudd.dev logo" /></a>
      </div>
      <div class="nav">
        <img src="images/icons/hamburger.svg" alt="menu icon" />
      </div>
    </div>
  </Container1200>
</header>

<style>
  header {
    height: 70px;
    padding-top: 64px;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .header-items {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>