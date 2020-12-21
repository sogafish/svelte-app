<script lang="ts">
  import Counter from './components/Counter.svelte';
  import Button from './components/Button.svelte';

  let count = 0;
  const incrementCount = () => {
    count += 1;
  };
</script>

<div>
  <Counter
    count={count}
  />
  <Button
    onClick={incrementCount} text='OnClick'
  />
</div>

<style>
</style>