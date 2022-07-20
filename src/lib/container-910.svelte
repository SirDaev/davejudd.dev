<script>
  let className = '';
  export { className as class };
</script>

<div class='{className}'>
  <slot />
</div>

<style>
  div {
    width: 100%;
    max-width: 910px;
    padding: 0 15px;
    margin: 0 auto;
  }
</style>