<!-- Plot.svelte -->
<svelte:head>
  <title>Plot</title>
  <meta name="description" content="About this Plot" />
</svelte:head>

<script>
  export let data;
</script>

<svg width="400" height="400">
  <g>
    <ul>
      {#each data.flowers as flower}
      <li>{flower.sepalLength}</li>
      {/each}
    </ul>
  </g>
</svg>
