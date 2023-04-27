<script>
  import { softwareAssests, soSimple, aFully } from "../constants";
  import HomeImg from "../homeImg.png";
  import Button from "./button.svelte";
  import TiLocationArrow from "svelte-icons/ti/TiLocationArrow.svelte";
</script>

<div class="grid grid-cols-3 pl-5 sm:pl-20 pr-0 bg-[#fdfdfd]">
  <div class="col-span-2 md:py-20 py-5">
    <h2 class="text-[#272727] font-bold text-lg sm:text-[40px] sm:leading-10">
      {@html softwareAssests} <span class="text-[#ff5c77]">{soSimple}</span>
    </h2>
    <p class="py-4 font-normal">{aFully}</p>
    <div class="flex justify-start items-center mt-3">
      <Button
        bgColor="#ff5c77"
        textColor="#ffffff"
        Class="px-6 py-1 rounded-2xl hover:scale-105  "
        ><a href="/">Book a Demo</a></Button
      >

      <a href="/" class="flex justify-start items-end mx-3"
        >Learn More <span class="w-6 mr-2"><TiLocationArrow width={30} /></span>
      </a>
    </div>
  </div>
  <div class="justify-items-end">
    <img src={HomeImg} alt="homeImage" width="350px" class="float-right" />
  </div>
</div>
