<script>
  export let icon = "";
  export let verb = "";
  export let explain = "";
  export let otherTxt = "";
</script>

<div class="">
  <div>
    <img src={icon} alt="main Icon">
  </div>
  <div>
    <p>{verb}</p>
    <p>{explain}</p>
    <p>{otherTxt}</p>
  </div>
</div>
