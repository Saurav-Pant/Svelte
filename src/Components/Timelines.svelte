<script>
  import first from "../assets/large01.jpeg";
  import Second from "../assets/02_img.png";
  import Timeline from "../assets/timeline.png";
  import Third from "../assets/03.jpeg";
  import Fourth from "../assets/04.png";
  import Timeline2 from "../assets/timeline2.png";
  import logo from "../assets/logo_small.png";
  import Picture from "./Picture.svelte";
</script>

<div>
  <div class="flex justify-center items-center gap-1 lg:gap-x-32 flex-wrap">
    <div>
      <img src={Timeline} alt="" />
    </div>
    <div class="flex justify-center gap-10 flex-wrap">
      <div>
        <Picture />
      </div>
      <div>
        <Picture />
      </div>
    </div>
  </div>
  <div></div>
</div>
<div class="flex justify-center items-center gap-1">
  <div>
    <img src={Timeline2} alt="" />
  </div>
  <div class="mx-auto mt-5 bg-gray-50 shadow-sm px-20 py-4 rounded-xl">
    <h1 class="text-xl font-bold">Co-Founder and CEO</h1>
    <p class="text-gray-400">Full-time Remote</p>
  </div>
</div>
