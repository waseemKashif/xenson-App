<script>
  import { madeBy, ItisSaid, cultureWise } from "../constants";
  import VideoImage from "../video.png";
  import TiLocationArrow from "svelte-icons/ti/TiLocationArrow.svelte";
</script>

<div
  class="sm:grid sm:grid-cols-2 gap-4 px-5 md:px-20 md:py-10 xl:py-20 xl:py-30 flex flex-col-reverse py-4 flex-wrap"
>
  <div class="flex flex-col">
    <h2 class="text-3xl font-semibold">{madeBy}</h2>
    <p class="sm:py-4 pt-1">{ItisSaid}</p>
    <p class="sm:py-2">{cultureWise}</p>
    <a href="/" class="flex justify-start items-end text-[#ff5c77]"
      >Learn More <span class="w-6 mr-2"><TiLocationArrow width={30} /></span>
    </a>
  </div>
  <div class=" md:py-4self-center">
    <img src={VideoImage} alt="videoIMG" class="w-max  cursor-pointer" />
  </div>
</div>
