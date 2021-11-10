<script>
  export let item;

</script>

<style>
  li {
    display: flex;
    flex-direction: column;

    margin-top: 1rem;
    margin-bottom: 1rem;
  }
</style>

<li class="search__result-normal search__result--item">
  <a href={item['@id']}>
    <span>{item['@type']}</span>
    <span>{item.Description}</span>
    <span>{item.Title}</span>
    <span>{item.description}</span>
    <span>{item.fhnw_location}</span>
    <span>{item.path_string}</span>
    <span>{item.portal_type}</span>
    <span>{item.review_state}</span>
    <span>{item.taxonomy_competence}</span>
    <span>{item.taxonomy_eduproducttype}</span>
    <span>{item.taxonomy_subjectarea}</span>
    <span>{item.taxonomy_title}</span>
  </a>
</li>