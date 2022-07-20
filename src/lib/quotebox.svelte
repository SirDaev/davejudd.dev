<script>
  export let centered = true;
</script>

<figure class="{centered === true ? 'centered' : ''}">
  <slot />
</figure>

<style>
  figure {
    background: #f5f5f5;
    width: 100%;
    max-width: 700px;
  }

  figure.centered {
    margin-left: auto;
    margin-right: auto;
  }
</style>