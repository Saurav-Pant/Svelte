<script>
  import BigPhoto from "../assets/Big Photo.png";
  import logo_small from "../assets/logo_small.png";
  import arrow from "../assets/arrow.png";
  import Threedot from "../assets/Threedot.png";

  let Followed = false;

  function toggle() {
    Followed = !Followed;
  }
</script>

<div
  class="flex flex-col lg:flex-row justify-evenly items-center mx-4 lg:mx-36 mt-10"
>
  <div class="flex flex-col gap-4 items-center">
    <img class="rounded-full" alt="pic" src={BigPhoto} />
    <p class="text-2xl text-center text-gray-500 mb-4">Krishna Kiran</p>
  </div>

  <div class="mb-6 lg:mb-0 mx-2">
    <p
      class="w-[60vw] lg:w-[37vw] text-sm font-sans text-gray-600 leading-5 lg:text-left"
    >
      Co-Founder and CEO at Duggup - Social network for people in tech.
      Ex-Amazon Head of Engineering. I write hot-takes on building a business,
      shipping delightful products and accelerating product and career growth.
    </p>
    <div class="flex justify-between items-center w-full relative md:top-5">
      <div>
        <button
          class={"w-[110px] outline outline-[0.5px] text-[#4D4D4D] px-5 py-2 rounded-md border-[#4D4D4D] hover:bg-[#0066FF] hover:border-blue-800 hover:outline-[#0066FF] hover:border-b-2 hover:text-white transition-all duration-200 "}
          on:click={toggle}
        >
          {#if Followed}
            Followed
          {:else}
            Follow
          {/if}
        </button>
      </div>
      <div class="flex flex-col items-center">
        <a href="/" class="flex justify-center lg:justify-start items-center">
          <span class="text-gray-500">My Website</span>
          <img src={arrow} alt="" class="ml-2 lg:ml-4" />
          <img src={Threedot} alt="" class="ml-2 lg:ml-6" />
        </a>
      </div>
    </div>
  </div>

  <div class="flex flex-col items-center md:items-end gap-1">
    <div class="">
      <a href="https://www.linkedin.com/in/duggup/">
        <img src={logo_small} alt="" class="ml-5" />
      </a>
      <p class="font-bold text-center lg:text-left">Duggup</p>
    </div>
    <p class="text-center lg:text-left text-gray-400">Co-Founder and CEO</p>
    <br />
  </div>
</div>
