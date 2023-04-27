<script>
  export let Class;
  export let bgColor = "blue";
  export let textColor = "white";
</script>


  <button
    class={Class}
    style="background-color: {bgColor}; color: {textColor}; "
    >
    <slot /></button
  >


<style>
  button {
    background-color: blue;
    color: white;
  }
</style>
