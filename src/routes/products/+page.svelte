<script>
  import NavBar from "$lib/navBar.svelte";
  import HomeLanding from "../../lib/homeLanding.svelte";
  import { ourProducts, ourFully, learnMore } from "../../constants";
  import productImg from "../../productsImg.png";
</script>

<div>
  <NavBar />
  <HomeLanding
    titleTxt={ourProducts}
    detailsTxt={ourFully}
    btnTxt={learnMore}
    HomeImg={productImg}
    Class="bg-gradient-to-t from-[#fbf0f2] grid grid-cols-3 pl-5 md:mt-24 mt-16 sm:pl-20 pr-0"
  />
</div>
