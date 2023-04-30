<script>
  export let titleText = "";
  export let bottomText = "";
  export let viewImg = "";
  export let Class = "";
</script>

<div class="flex flex-col sm:grid sm:grid-cols-2 bg-[#fd6379]  gap-0 {Class}">
  <div class=" flex py-20 sm:py-0 flex-col text-white justify-center text-center ">
    <div class=" md:px-2 items-start  sm:py-0 px-5 w-auto">
      <p class="text-4xl">"{titleText} "</p>
    </div>
    <p>{bottomText}</p>
  </div>
  <div>
    <img src={viewImg} alt={bottomText} class="w-full" />
  </div>
</div>
