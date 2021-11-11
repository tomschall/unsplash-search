<script>
  import { _ } from 'svelte-i18n';
  import ListItem from './ListingNormal.svelte';
  import SearchCategories from './SearchCategories.svelte';

  export let results;
</script>

<div class="search__results">
  <div class="widg_searchbar-bar__title">{$_('searchresult_title')}</div>
  <div class="widg_searchbar-bar__content custom-scrollbar" data-searchbar="content">
    <SearchCategories />
    <div class="search__cat">
      <ul class="search-results">
        {#each results as result (result)}
        <ListItem item={result} />
        {/each}
      </ul>
    </div>
  </div>
</div>
