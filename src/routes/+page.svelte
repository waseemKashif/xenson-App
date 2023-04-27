<script>
  import NavBar from "../components/navBar.svelte";
  import HomeLanding from "../components/homeLanding.svelte";
  import VideoIntro from "../components/videoIntro.svelte";
  import Title from "../components/title.svelte";
  import PristonIcon from "../prtison.png";
  import NorthIcon from "../northWali.png";
  import OldMuthal from "../oldMuthal.png";
  import SveskaIcon from "../svenska.png";
  import SvekoIcon from "../sweko.png";
  import IconsList from "../components/iconsList.svelte";
  import DetailedList from "../components/detailedList.svelte";

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
</div>
