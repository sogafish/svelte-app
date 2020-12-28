<script lang="ts">
  export let placeholder: string;
  export let value: string;
</script>

<div class="input-text">
  <input placeholder={placeholder} bind:value={value} >
</div>

<style>
</style>
