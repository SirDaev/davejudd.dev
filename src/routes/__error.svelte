<script>
  import Container1200 from "$lib/container-1200.svelte";
</script>

<section id="not-found">
  <div class="content text-center">
    <Container1200>
      <h1 class="big-title">
        <span>404</span><br />Page not found.
      </h1>
      <ul class="links">
        <li>
          <a href="/">Home</a>
        </li>
      </ul>
    </Container1200>
  </div>
</section>

<style>
  .content {
    padding: 80px 0;
  }

  @media (min-width: 992px) {
    .content {
      padding: 150px 0;
    }
  }

  .big-title {
    font-size: 6rem;
    line-height: 1;
    font-weight: 400;
    margin-bottom: 60px;
  }

  .big-title span {
    font-weight: 600;
    font-size: 1.2em;
  }

  .links {
    margin: 20px 0;
  }

  .links a {
    font-size: 2.5rem;
  }
</style>