<script>
  export let itemList = [];
</script>

<div>
  <ul class="flex flex-col px-5">
    {#each itemList as item (item)}
      <li class="text-sm md:text-base cursor-pointer">
        <a
          href={item.link}
          class=" whitespace-nowrap text-[#878787] hover:text-[#585555]"
          >{item.name}</a
        >
      </li>
    {/each}
  </ul>
</div>
