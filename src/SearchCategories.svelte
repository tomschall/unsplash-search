<script>
  import { _ } from 'svelte-i18n';

  export let prop;

  // const getCategory = (e) => {
  //   e.preventDefault();
  //   const str = e.target.innerText;
  //   const category = str.split(' ');
  //   const currentCategory = category[0];
  //   console.log(categorySelected);
  //   dispatch('value', { text: currentCategory })
  // }

</script>

<div class="widg_searchbar-bar__categories" data-searchbar="cat" style="display: flex;">
  <button class="button button__cat active" on:click={() => prop = 'all'}>
    {$_('category_all')} (2562)
  </button>
  <button class="button button__cat" on:click={() => prop = 'studiengänge'}>
    {$_('category_studys')} (1000)
  </button>
  <button class="button button__cat" on:click={() => prop = 'weiterbildungsangebot'}>
    {$_('category_education')} (15)
  </button>
  <button class="button button__cat" on:click={() => prop = 'events'}>
    {$_('category_events')} (1)
  </button>
  <button class="button button__cat" on:click={() => prop = 'news'}>
    {$_('category_news')} (53)
  </button>
  <button class="button button__cat" on:click={() => prop = 'dokumente'}>
    {$_('category_documents')} (1946)
  </button>
  <button class="button button__cat" on:click={() => prop = 'personen'}>
    {$_('category_persons')} (26)
  </button>
  <button class="button button__cat" on:click={() => prop = 'allgemein'}>
    {$_('category_general')} (504)
  </button>
  <button class="button button__cat ref">&nbsp;&nbsp;</button>
</div>