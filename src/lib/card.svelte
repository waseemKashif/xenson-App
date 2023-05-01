<script>
  import TiLocationArrow from "svelte-icons/ti/TiLocationArrow.svelte";
    export let videoImage = '';
    export let title = '';
    export let details= '';
    export let link ='';

</script>

<div class="flex flex-col bg-[#f9f9f9] rounded-xl mb-6 pb-4">
    
       <img src={videoImage} alt={title} class="w-full self-center cursor-pointer">
    
    <div class=" flex flex-col sm:px-4 px-2">

        <p class="self-center sm:self-start text-2xl font-medium py-4">{title}</p>
        <p class="self-center text-[#bfbfbf] text-sm pb-4">
            {details}
        </p>
        <a href="/" class="flex justify-start items-end  whitespace-nowrap self-center sm:self-start text-[#ff5c77]"
            >{link} <span class="w-6 mr-2"><TiLocationArrow width={30} /></span>
          </a>
    </div>
      <slot></slot>
</div>