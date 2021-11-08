<script>
  import PhotoCard from './PhotoCard.svelte';

  export let results;
</script>

<ul class="search-results">
  {#each results as result (result.id)}
    <PhotoCard photo={result} />
  {/each}
</ul>
