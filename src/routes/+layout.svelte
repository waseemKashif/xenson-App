<script>
  import Navbar from "$lib/navBar.svelte";
  import "../app.css";
  import Footer from "$lib/footer.svelte";
  import Logo from "../logoSRC.png";
  import {
    itemList1,
    itemList2,
    itemList3,
    itemList4,
  } from "../routes/products/products.mocks";
</script>

<header>
  <Navbar />
</header>
<main>
  <slot />
</main>
<footer>
  <Footer
    listItems={[itemList1, itemList2, itemList3, itemList4]}
    logo={Logo}
  />
</footer>
