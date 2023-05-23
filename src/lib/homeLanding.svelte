<script>
  import Button from "./button.svelte";
  import TiLocationArrow from "svelte-icons/ti/TiLocationArrow.svelte";
  export let titleTxt = "";
  export let highlighTxt = "";
  export let detailsTxt = "";
  export let HomeImg = "";
  export let btnTxt = "";
  export let Class = "";
  export let linkTxt = "";
  export let detailClass = "";
</script>

<div class={Class}>
  <div class="col-span-2 md:mt-10 md:py-20 py-5">
    <h2
      class="text-[#272727] font-bold text-lg sm:text-2xl md:text-[40px] sm:leading-10"
    >
      {@html titleTxt}
      {#if highlighTxt}
        <span class={detailClass}>{highlighTxt}</span>
      {/if}
    </h2>
    {#if detailsTxt}
      <p class="py-4 text-sm sm:text-lg sm:w-[80%]">{detailsTxt}</p>
    {/if}
    <div class="flex justify-start items-center mt-3">
      <Button
        bgColor="#ff5c77"
        textColor="#ffffff"
        Class="sm:px-6 px-4 text-sm sm:text-base py-1 rounded-2xl hover:scale-105  "
        ><a href="/" class=" whitespace-nowrap">{btnTxt}</a></Button
      >
      {#if linkTxt}
        <a
          href="/"
          class="flex justify-start items-end mx-3 whitespace-nowrap text-sm sm:text-base"
          >{linkTxt}
          <span class="w-6 mr-2"><TiLocationArrow /></span>
        </a>
      {/if}
    </div>
  </div>
  <div class="justify-items-end">
    <img src={HomeImg} alt="homeImage" class="float-right w-full h-full" />
  </div>
</div>
