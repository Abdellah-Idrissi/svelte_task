
<script>
  import MousePointer2 from 'lucide-svelte/icons/mouse-pointer-2';
</script>


<div class="px-5 lg:px-7 py-4 xl:py-5 fixed xl:sticky bottom-0 border-t border-[#2E3032] w-full bg-[#252628]">
  <div class="relative ">

    <input type="text" placeholder="Start a searching..." class="bg-[#161719] placeholder:text-neutral-500 placeholder:text-sm sm:placeholder:text-[14.5px] lg:placeholder:text-[15px] w-full rounded-lg h-8 sm:h-12 text-neutral-500 p-3 lg:px-4 py-5 lg:py-[25px] outline-none border-none text-sm sm:text-[14.5px] lg:text-[15px]  ">

    <div class="absolute right-3 lg:right-4 top-[51%] -translate-y-1/2 bg-[#161719] cursor-pointer">
      <MousePointer2 color={'#ffff'} class={'w-4 h-4 sm:w-[18px] sm:h-[18px] lg:h-5 lg:w-5 rotate-[136deg]'} />
    </div>

  </div>
  
</div>