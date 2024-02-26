<script>
  import HelpCircle from 'lucide-svelte/icons/help-circle';
  import Search from 'lucide-svelte/icons/search';
  import Grid2X2 from 'lucide-svelte/icons/grid-2x2';
  import Settings from 'lucide-svelte/icons/settings';
  import LogOut from 'lucide-svelte/icons/log-out';
  import profile from "../images/profile.jpg"
  import gpt from "../images/gpt.png"
  import Plus from 'lucide-svelte/icons/plus';
</script>

<div class="px-7 py-5 border-r border-[#2E3032] flex flex-col bg-[#161719]">
  <div>
    <div class='flex gap-x-1 items-end mt-2'>
      <img src={gpt} alt="gpt" class="w-10 h-10">
      <p class="montserrat tracking-tight text-[#03c275] text-4xl">OpenAI</p>
    </div>
  </div>

  <div class="flex-1 flex flex-col justify-between ">

    <div class="my-[70px] w-full">

      <button class="bg-[#48DF7E] w-full py-[11px] rounded-lg flex items-center gap-x-3 justify-center">
        <Plus size={20} />
        <span class="font-semibold">New Thread</span>
      </button>

      <div class="mt-[60px]">
        <div class="flex flex-col gap-y-5">

          <div class="flex flex-col gap-y-5 border-b border-[#2E3032] pb-5">
            <div class="flex gap-x-3 items-center">
              <HelpCircle size={22} class='text-blue-700' />
              <p class="text-white">Guide & FAQ</p>
            </div>
  
            <div class="flex gap-x-3 items-center">
              <Search size={22} class='text-[#03c275]' />
              <p class="text-white">Search</p>
            </div>
          </div>

          <div class="flex flex-col gap-y-5 border-b border-[#2E3032] pb-5">
            <div class="flex gap-x-3 items-center">
              <Grid2X2 size={22} class='text-orange-700' />
              <p class="text-white">Upgrade</p>
            </div>
  
            <div class="flex gap-x-3 items-center">
              <Settings size={22} class='text-indigo-700' />
              <p class="text-white">Setting</p>
            </div>
          </div>

          <div class="flex flex-col gap-y-5  pb-5">
            <div class="flex gap-x-3 items-center">
              <LogOut size={22} class='text-pink-200'/>
              <p class="text-white">Log out</p>
            </div>
  

        </div>


        </div>
      </div>

    </div>

    <div class="bg-[#252628] rounded-2xl p-5 ">

      <div class="flex gap-x-[10px] items-center">
        <div><img src={profile} alt="profile" class="w-14 h-14 rounded-full"></div>

        <div class="text-sm flex-1">
          <div class="flex justify-between items-center mb-1">
            <p class="font-semibold text-white">Arjun Makwana</p>
            <div class="bg-blue-500 text-white py-[2px] px-[10px] rounded-md text-xs">Free</div>
          </div>

          <div class="text-neutral-500">arjunmakwana@gmail.com</div>
        </div>

      </div>

      <button class="p-4 border border-neutral-600 text-white grid place-content-center font-medium rounded-xl mt-7 w-full">
        Upgrade to Pro
      </button>

    </div>

  </div>
</div>