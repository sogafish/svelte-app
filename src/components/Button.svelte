<script lang="ts">
  let onClick: () => void;
  let text: string = 'Click';

  export {
    onClick,
    text,
  };
</script>

<button on:click={onClick}>{text}</button>
