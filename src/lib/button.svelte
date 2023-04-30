<script>
  export let Class;
  export let bgColor = "#fd6379";
  export let textColor = "#ffffff";
</script>


  <button
    class="   {Class}"
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
