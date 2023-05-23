<script>
  import DetailedItem from "./detailedItem.svelte";
  import RatingBox from "./ratingBox.svelte";
  import Button from "./button.svelte";

  import Detail_1 from "../samIcon.png";
  import Detail_2 from "../detail-2.png";
  import Detail_3 from "../detail-3.png";
  import {
    simplifyYour,
    withXansam,
    theStrongest,
    xensonHas,
    oneSam,
    atXenson,
    enterpriseIn,
    theTrue,
    inRating,
    inRatingOn,
    presented,
    onAverage,
    theAverage,
  } from "../constants";
</script>

<div class="sm:py-20">
  <DetailedItem
    Class="sm:grid sm:grid-cols-2 flex flex-col md:px-20 px-5 gap-4 items-center"
    IconImage={Detail_1}
    title={simplifyYour}
    detail={withXansam}
  />
  <DetailedItem
    Class="sm:grid sm:grid-cols-2 flex flex-col-reverse md:px-20 px-5 gap-4 items-center"
    IconImage={Detail_2}
    title={theStrongest}
    detail={xensonHas}
    reverse="true"
  />
  <DetailedItem
    Class="sm:grid sm:grid-cols-2 gap-4 flex flex-col md:px-20 px-5 items-center"
    IconImage={Detail_3}
    title={oneSam}
    detail={atXenson}
  />
  <div
    class="flex my-6 flex-col-reverse items-center sm:items-start sm:pt-8 pt-5 sm:grid sm:grid-cols-2 gap-4 md:px-20 px-5"
  >
    <DetailedItem
      Class=" flex flex-col "
      title={enterpriseIn}
      detail={theTrue}
      reverse="true"
    >
      <Button
        bgColor="#ff5c77"
        textColor="#ffffff"
        Class="px-6 py-1 rounded-2xl hover:scale-105 sm:w-fit mt-4 "
        ><a href="/" class=" whitespace-nowrap">Book a Demo</a></Button
      >
    </DetailedItem>
    <div class="flex flex-col items-center sm:items-start">
      <div class="flex gap-2 sm:col-span-1">
        <div class="flex h-fit justify-center mr-16">
          <span class=" bg-[#ff5c77] w-[3px] h-auto justify-evenly mr-10" />
          <span
            class="text-[#ff5c77] sm:text-7xl text-5xl font-bold sm:mb-6 mb-5"
            >950 <span class="sm:text-5xl text-3xl absolute">%</span></span
          >
        </div>

        <div class="font-semibold">
          <p class=" whitespace-nowrap">{presented} <br />{onAverage}</p>
        </div>
      </div>
      <div>
        <div class="flex mt-4 gap-5">
          <RatingBox rating="4.9" maxRating="5" details={inRatingOn} />
          <div>
            <RatingBox rating="5" maxRating="5" details={inRating} />
          </div>
        </div>
      </div>
      <p class=" text-xs">{theAverage}</p>
    </div>
  </div>
</div>
