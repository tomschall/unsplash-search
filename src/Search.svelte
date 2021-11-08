<script>
  export let query;
  export let handleSubmit;
</script>

<form on:submit|preventDefault={handleSubmit}>
  <div class="widg_searchbar-bar__search">
    <div class="widg_searchbar-bar__close" data-searchbar="close"></div>
    <label for="search" class="visuallyhidden">Search: </label>
    <input bind:value={query} type="text" name="searchbar_search" data-searchbar="input"/>
  </div>
</form>
