<script lang="ts">
  import * as Sheet from "$lib/components/ui/sheet";
  import profile from "../images/profile.jpg"
  import gpt from "../images/gpt.png"
  import Trash2 from 'lucide-svelte/icons/trash-2';
  import { Checkbox } from "$lib/components/ui/checkbox";
  import Plus from 'lucide-svelte/icons/plus';


</script>

<Sheet.Root>

  <Sheet.Trigger class='grid place-content-center'>
    <button class="w-6 h-6 rounded-full bg-[#6AF39B]"></button>
  </Sheet.Trigger>


  <Sheet.Content class='w-[101%] 5s:!w-[380px] scrollbar-thin scrollbar-track-neutral-800 scrollbar-thumb-neutral-700  bg-[#171717] border-none outline-none overflow-y-auto flex flex-col '>

    <Sheet.Header>
      <Sheet.Title class='mt-5 border-b border-neutral-700 pb-6'>

        <div class="flex gap-x-5 items-center">

          <div class="relative">
            <img src={profile} alt="profile" class="w-14 h-14 rounded-full border border-white/10 ">
            <div class="absolute bottom-1 right-1 bg-green-400 w-2 h-2 rounded-full"></div>
          </div>
          <button class="bg-[#8D55EA] py-[10px] px-6 text-white font-medium text-sm rounded-md">
            Upgrade to Pro
          </button>

        </div>

      </Sheet.Title>
    </Sheet.Header>

    <div class="flex-1 mt-3 flex flex-col gap-y-6">

      <div class="flex justify-between items-center">
        <div class="flex gap-x-2 items-center">
          <p class="text-neutral-500 text-sm font-semibold">Chat History</p>
          <div class="bg-[#2A2F30] text-xs p-2 py-1 rounded-md text-neutral-500 font-semibold">25/100</div>
        </div>

        <div><Trash2 size={17} class='text-neutral-500' /></div>
      </div>

      <div class="w-full rounded-md bg-[#343839] p-5 flex flex-col gap-y-[20px]">
        <div class="flex items-center justify-between">
          <Checkbox id="terms" class={'border border-neutral-600 h-6 w-6 '} />
          <p class="text-neutral-500 text-sm">Just now</p>
        </div>

        <div class="flex flex-col gap-y-[9px] ">
          <div class="text-white font-bold text-lg leading-none">AI now a days</div>
          <p class="text-neutral-500 text-sm leading-relaxed">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint iusto a ad incidunt voluptas eaque aliquid nam vitae quibusdam hic id quisquam animi, eos, ea vero, amet veritatis esse nobis.</p>
          <div><img src={profile} alt="profile" class="w-10 h-10 rounded-full"></div>
        </div>
      </div>

      <div class="w-full rounded-md  p-5 flex flex-col gap-y-[20px]">
        <div class="flex items-center justify-between">
          <Checkbox id="terms" class={'border border-neutral-600 h-6 w-6 '} />
          <p class="text-neutral-500 text-sm">Just now</p>
        </div>

        <div class="flex flex-col gap-y-[9px] ">
          <div class="text-white font-bold text-lg leading-none">Welcome to ChatGPT</div>
          <p class="text-neutral-500 text-sm leading-relaxed">Hello! How can I assist you ?</p>

          <div class="bg-[#343839] h-[100px] grid place-content-center rounded-md">
            <div class='flex gap-x-1 items-end '>
              <img src={gpt} alt="gpt" class="w-10 h-10">
              <p class="montserrat tracking-tight text-[#03c275] text-4xl leading-none">OpenAI</p>
            </div>
          </div>

          <div><img src={profile} alt="profile" class="w-10 h-10 rounded-full"></div>
        </div>
      </div>

      <div class="w-full rounded-md p-5 flex flex-col gap-y-[20px]">
        <div class="flex items-center justify-between">
          <Checkbox id="terms" class={'border border-neutral-600 h-6 w-6 '} />
          <p class="text-neutral-500 text-sm">Just now</p>
        </div>

        <div class="flex flex-col gap-y-[9px] ">
          <div class="text-white font-bold text-lg leading-none">Auto Generate Title</div>
          <p class="text-neutral-500 text-sm leading-relaxed">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint iusto a ad incidunt voluptas eaque aliquid.</p>
          <div><img src={profile} alt="profile" class="w-10 h-10 rounded-full"></div>
        </div>
      </div>

      <button class="bg-[#48DF7E] w-full py-[11px] rounded-lg flex items-center gap-x-3 justify-center mt-8 mb-2 ">
        <Plus size={20} />
        <span class="font-semibold">New Thread</span>
      </button>

    </div>

  </Sheet.Content>

</Sheet.Root>