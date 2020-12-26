<script lang="ts">
  import { list } from '../stores';

  let _list;

  const unsubscribe = list.subscribe(value => {
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
