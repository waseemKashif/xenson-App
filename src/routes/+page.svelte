<script>
  import NavBar from "$lib/navBar.svelte";
  import HomeLanding from "$lib/homeLanding.svelte";
  import VideoIntro from "$lib/videoIntro.svelte";
  import Title from "$lib/title.svelte";
  import PristonIcon from "../prtison.png";
  import NorthIcon from "../northWali.png";
  import OldMuthal from "../oldMuthal.png";
  import SveskaIcon from "../svenska.png";
  import SvekoIcon from "../sweko.png";
  import Larki from "../larki.png"
  import IconsList from "$lib/iconsList.svelte";
  import DetailedList from "$lib/detailedList.svelte";
  import TitleWithImage from "../lib/titleWithImage.svelte";
  import {weCould,mariaBer,whatIs} from "../constants"

  let Icons = [PristonIcon, OldMuthal, SvekoIcon, NorthIcon, SveskaIcon];
  
</script>

<div class="">
  <NavBar />
  <HomeLanding />
  <VideoIntro />
  <Title
    Class="md:text-xl sm:text-lg text-base text-center text-[#727272] sm:py-4"
    >Global Trust For Xensam</Title
  >
  <IconsList
    {Icons}
    Class="flex items-center justify-between flex-wrap sm:px-20 px-5"
  />
  <DetailedList/>
  <TitleWithImage Class="sm:grid sm:grid-cols-2   " titleText={weCould} bottomText={mariaBer} viewImg={Larki}  />
  <Title Class="text-center text-4xl font-medium sm:mt-10 mt-6" >{whatIs}</Title>
</div>
