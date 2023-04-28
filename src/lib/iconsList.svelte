<script>
  export let Class = "";
  export let Icons = [];
</script>

<div class={Class}>
  {#each Icons as icon (icon)}
    <img src={icon} alt="ListIcon" />
  {/each}
</div>
