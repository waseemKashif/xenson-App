<script>
  import Logo from "../logoSRC.png";
  import Button from "./button.svelte";
</script>

<nav class="grid grid-cols-4 gap-4 py-6 items-center px-5 sm:px-20">
  <div class="col-span-1 items-center">
    <img src={Logo} alt="logo" class="cursor-pointer" />
  </div>
  <div class="col-span-3 text-md font-semibold">
    <ul class="flex justify-evenly items-center">
      <li class="hover:scale-105"><a href="/products">Products</a></li>
      <li class="hover:scale-105"><a href="/">Solutions</a></li>
      <li class="hover:scale-105"><a href="/">About Us</a></li>
      <li class="hover:scale-105"><a href="/">Contact Us</a></li>
      
      <li>
        <Button
          textColor="#fe647e"
          bgColor="#fae7eb"
          Class="px-6 py-1 rounded-2xl hover:scale-105 "
          ><a href="/">Book a Demo</a></Button
        >
      </li>
    </ul>
  </div>
</nav>
