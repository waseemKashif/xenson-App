<script>
  export let IconImage = null;
  export let title = "";
  export let detail = "";
  export let Class = "";
  export let reverse = false;
</script>

<div class={Class}>
  {#if !reverse}
    {#if IconImage != null}
      <img src={IconImage} alt="title" />
    {/if}

    <div class="flex flex-col">
      <p class="md:text-3xl sm:text-2xl text-xl sm:py-4 py-1 font-semibold">
        {title}
      </p>
      <p>{detail}</p>
    </div>
  {:else}
    <div class="flex flex-col">
      <p class="md:text-3xl sm:text-2xl text-xl sm:py-4 py-1 font-semibold">
        {title}
      </p>
      <p>{detail}</p>
    </div>
    {#if IconImage != null}
      <img src={IconImage} alt="title" />
    {/if}
  {/if}

  <slot />
</div>
