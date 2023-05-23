<script>
  import HomeLanding from "$lib/homeLanding.svelte";
  import VideoIntro from "$lib/videoIntro.svelte";
  import Title from "$lib/title.svelte";
  import IconsList from "$lib/iconsList.svelte";
  import DetailedList from "$lib/detailedList.svelte";
  import TitleWithImage from "$lib/titleWithImage.svelte";
  import PristonIcon from "../prtison.png";
  import NorthIcon from "../northWali.png";
  import OldMuthal from "../oldMuthal.png";
  import SveskaIcon from "../svenska.png";
  import SvekoIcon from "../sweko.png";
  import Larki from "../larki.png";
  import card1 from "../cardimg.png";
  import card2 from "../cardimg1.png";
  import card3 from "../cardimg2.png";
  import HomeImg from "../homeImg.png";
  import Card from "$lib/card.svelte";
  import {
    weCould,
    mariaBer,
    whatIs,
    latestBk,
    samsEurope,
    newsLetter,
    newsVideo,
    softwareAssests,
    soSimple,
    aFully,
    learnMore,
    bookAdemo,
  } from "../constants";

  const Icons = [PristonIcon, OldMuthal, SvekoIcon, NorthIcon, SveskaIcon];

</script>

<div class="">
  <!-- <NavBar /> -->
  <HomeLanding
    {HomeImg}
    titleTxt={softwareAssests}
    highlighTxt={soSimple}
    detailsTxt={aFully}
    linkTxt={learnMore}
    btnTxt={bookAdemo}
    Class="grid grid-cols-3 pl-5 md:mt-24 mt-16 sm:pl-20 pr-0 bg-[#fdfdfd]"
    detailClass="text-[#ff5c77]"
  />
  <VideoIntro />
  <Title
    Class="md:text-xl sm:text-lg text-base text-center text-[#727272] sm:py-4"
    >Global Trust For Xensam</Title
  >
  <IconsList
    {Icons}
    Class="flex items-center justify-between flex-wrap sm:px-20 px-5"
  />
  <DetailedList />
  <TitleWithImage
    Class="sm:grid sm:grid-cols-2   "
    titleText={weCould}
    bottomText={mariaBer}
    viewImg={Larki}
  />
  <Title Class="text-center text-4xl font-medium sm:mt-10 mt-6">{whatIs}</Title>
  <div
    class="md:grid md:grid-cols-3 sm:px-20 px-5 flex w-maz flex-col items-center sm:grid-cols-2 sm:grid md:gap-4 sm:gap-2 sm:mt-10 md:mt-14"
  >
    <Card
      title={newsLetter}
      details={latestBk}
      videoImage={card2}
      link="Read More"
    />
    <Card
      title={newsVideo}
      details={latestBk}
      videoImage={card3}
      link="Read More"
    />
    <Card
      title={samsEurope}
      details={latestBk}
      videoImage={card1}
      link="Read More"
    />
  </div>
</div>
