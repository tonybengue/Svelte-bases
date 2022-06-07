<script>
  let count = 0

  function addOne() {
    count++
  }
</script>

<button on:click={addOne}>Clicked {count} times</button>

{#if count > 5}
  <p>Good Job</p>

  {#each ['🤣', '😊', '😍'] as face}
    <p>Hello {face}</p>
  {/each}
{/if}
