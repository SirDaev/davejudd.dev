<script>
  let type = 'link';
</script>

{#if type === 'link'}
	<div class="button">
    <slot />
  </div>
{/if}

<style>
  .button {
    display: inline-block;
    background: #337AB7;
    color: #fff;
    font-size: 1.9rem;
    font-weight: 600;
    padding: 15px 30px;
    border-radius: 6px;
    cursor: pointer;
    transition: background-color .1s ease-out;
  }

  .button:hover {
    background-color: #F7ACD4;
  }
</style>