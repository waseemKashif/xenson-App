<script>
  import { madeBy, ItisSaid, cultureWise } from "../constants";
  import VideoImage from "../video.png";
  import TiLocationArrow from "svelte-icons/ti/TiLocationArrow.svelte";
</script>

<div
  class="md:grid sm:grid-cols-12 px-5 sm:px-20 md:py-10 xl:py-20 md:py-30 flex flex-col-reverse py-4"
>
  <div class="col-start-1 sm:col-span-6">
    <h2 class="text-3xl font-semibold">{madeBy}</h2>
    <p class="sm:py-4 pt-1">{ItisSaid}</p>
    <p class="sm:py-2">{cultureWise}</p>
    <a href="/" class="flex justify-start items-end text-[#ff5c77]"
      >Learn More <span class="w-6 mr-2"><TiLocationArrow width={30} /></span>
    </a>
  </div>
  <div class="sm:col-start-8 sm:col-span-5 md:py-4">
    <img src={VideoImage} alt="videoIMG" class="w-200 h-200" />
  </div>
</div>
