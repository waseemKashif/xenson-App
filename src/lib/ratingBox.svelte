<script>
  export let rating = "";
  export let maxRating = "";
  export let details = "";
</script>

<div
  class="py-6 px-6 text-center border-dotted border-2 rounded-md border-gray-200 my-2 sm:my-8"
>
  <div class="flex justify-center items-center">
    <p class="text-[#ff5c77] sm:text-6xl text-5xl font-bold">{rating}</p>
    <p
      class=" mt-6 sm:mt-8 text-[#bfbfbf] text-3xl sm:text-[38px] font-bold scale-110 z-[-1]"
    >
      /{maxRating}
    </p>
  </div>

  <p class="w-min sm:px-4">
    {details}
  </p>

  <slot />
</div>
