<script>
  import { _ } from 'svelte-i18n';

  export let triggerCategorySearch = () => {};
  export let prop;
</script>

<div
  class="widg_searchbar-bar__categories"
  data-searchbar="cat"
  style="display: flex;"
>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'all';
      triggerCategorySearch();
    }}
  >
    {$_('category_all')} (2562)
  </button>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'studiengänge';
      triggerCategorySearch();
    }}
  >
    {$_('category_studys')} (1000)
  </button>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'weiterbildungsangebot';
      triggerCategorySearch();
    }}
  >
    {$_('category_education')} (15)
  </button>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'events';
      triggerCategorySearch();
    }}
  >
    {$_('category_events')} (1)
  </button>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'news';
      triggerCategorySearch();
    }}
  >
    {$_('category_news')} (53)
  </button>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'dokumente';
      triggerCategorySearch();
    }}
  >
    {$_('category_documents')} (1946)
  </button>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'personen';
      triggerCategorySearch();
    }}
  >
    {$_('category_persons')} (26)
  </button>
  <button
    class="button button__cat"
    on:click={() => {
      prop = 'allgemein';
      triggerCategorySearch();
    }}
  >
    {$_('category_general')} (504)
  </button>
  <button class="button button__cat ref">&nbsp;&nbsp;</button>
</div>
