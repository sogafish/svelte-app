<script lang="ts">
  import { list } from '../stores';

  type List = string[]

  let _list: List;

  list.subscribe((value: List) => {
    _list = value;
  });

</script>

<ul class="list-display">
  {#each _list as item}
    <li>{item}</li>
  {/each}
</ul>

<style>
</style>
