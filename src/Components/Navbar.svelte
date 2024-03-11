<script>
  import logo from "../assets/logo.png";
  import profile from "../assets/profile.png";
  import Home from "../assets/HomeIcon.png";
  import Explore from "../assets/Explore.png";
  import Learn from "../assets/Learn.png";
  import PostPlus from "../assets/PostPlus.png";
  import DownIcon from "../assets/DownIcon.png";
  let isMobileMenuOpen = false;
</script>

<div class="flex justify-around items-center py-3 border-b-2 border-dashed">
  <a href="/">
    <img src={logo} alt="logo" class="h-8 w-auto" />
  </a>
  <div class="flex items-center lg:hidden">
    <button class="text-gray-500 focus:outline-none">
      <svg
        class="h-6 w-6"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 12h16m-7 6h7"
        ></path>
      </svg>
    </button>
  </div>

  {#if !isMobileMenuOpen}
    <div class="flex items-center hidden lg:flex">
      <ul class="flex space-x-10">
        <a href="/">
          <li class="flex items-center space-x-2">
            <img src={Home} alt="" class="h-4 w-4" />
            <p class="text-gray-500">Home</p>
          </li>
        </a>
        <a href="/">
          <li class="flex items-center space-x-2">
            <img src={Explore} alt="" class="h-4 w-4" />
            <p class="text-gray-500">Explore</p>
          </li>
        </a>
        <a href="/">
          <li class="flex items-center space-x-2">
            <img src={Learn} alt="" class="h-4 w-4" />
            <p class="text-gray-500">Learn</p>
          </li>
        </a>
      </ul>

      <button
        class="outline outline-[0.5px] text-gray-500 py-1 rounded border-gray-100 border-2 px-3 mx-16 flex justify-center items-center border-b-gray-800 hidden lg:flex"
      >
        <img src={PostPlus} alt="" class="pr-2" />
        Post
      </button>
      <a href="/" class="hidden lg:flex">
        <div class="flex items-center">
          <div class="border-2 border-gray-400 rounded-full">
            <img src={profile} alt="" class="h-8 w-8 rounded-full" />
          </div>
          <h3 class="text-gray-800 px-4">Krishna Kiran</h3>
          <img src={DownIcon} alt="DownIcon" />
        </div>
      </a>
    </div>
  {:else}
    <div class="lg:hidden"></div>
  {/if}
</div>
