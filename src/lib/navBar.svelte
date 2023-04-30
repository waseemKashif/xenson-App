<script>
  import Logo from "../logoSRC.png";
  import Button from "./button.svelte";

  const list = [
    { name: "Products", link: "/products" },
    { name: "Solutions", link: "/" },
    { name: "About Us", link: "/" },
    { name: "Contact Us", link: "/" },
  ];

  $: open = false;

  const handleClick=()=> {
   open=!open
   console.log("button clicked..." ,open);
  }
</script>

<div class=" w-full fixed top-0 left-0 bg-[#fff]">
  <nav class=" md:flex py-6 items-center justify-between px-5 md:px-20">
    <div class="items-center">
      <img
        src={Logo}
        alt="logo"
        class="cursor-pointer rounded-md md:rounded-none"
      />
    </div>
    <div class="col-span-3 text-md font-semibold">
      <button
        class="absolute top-6 right-8 cursor-pointer md:hidden" 
       on:click={handleClick}
      >
      <ion-icon name={open ? "close" : "menu"} class="text-2xl visible md:invisible"  />
      
      
      </button>
      <ul
        class="md:flex justify-evenly md:items-center absolute md:static bg-[#fff] md:z-auto z-[-1] left-0 w-full md:w-auto pl-10 md:pl-0 pb-8 md:pb-0 transition-all duration-500 ease-in {open ? "top-16" : "top-[-490px]"}"
      >
        {#each list as link (link.name)}
          <li
            class="md:ml-8 md:hover:scale-105 hover:translate-x-1 duration-200 md:my-0 my-7"
          >
            <a href={link.link} class="whitespace-nowrap">{link.name}</a>
          </li>
        {/each}

        <Button
          textColor="#fe647e"
          bgColor="#fae7eb"
          Class="md:px-6 md:py-1 px-3  md:ml-8 whitespace-nowrap rounded-2xl hover:scale-105 "
          ><a href="/">Book a Demo</a></Button
        >
      </ul>
    </div>
  </nav>
</div>

<style>
 .ion-icon{
  visibility: visible;
 }
</style>
