<script>
  export let listItems = {};
  export let logo = "";
  import ServicesList from "./servicesList.svelte";
  import { xensamAB, privacyPolicy } from "../constants";
</script>

<div
  class="sm:grid sm:grid-cols-3 px-5 md:px-20 md:py-10 py-5 flex flex-col sm:items-start gap-5 mt-4"
>
  <div class=" self-center sm:self-start">
    <img src={logo} alt="itemLogo" class="" />
  </div>
  <div class=" grid grid-cols-4 gap-2 sm:col-span-2">
    {#each listItems as item (item)}
      <ServicesList itemList={item} />
    {/each}
  </div>
</div>
<div
  class="flex justify-between px-5 md:px-20 text-[10px] md:text-xs font-medium md:py-10"
>
  <p>{xensamAB}</p>
  <p>{privacyPolicy}</p>
</div>
