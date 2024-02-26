
<script lang="ts">
  import profile from "../images/profile.jpg"
  import gpt from "../images/gpt.png"

  const gptchats : {title:string, msg:string}[] = [
    {title:'Personalisation',msg:'AI personalization uses a customer’s demographic and past behavioral data such as browsing and purchasing history, as well as social media interactions to learn about the specific needs and preferences of that individual.'},

    {title:'User Testing',msg:'AI take care of repetitive tasks, speeding up the research process and letting your team focus on the exciting part discovering deeper insights, socializing key findings, and influencing strategic decisions.'},

    {title:'Content creation',msg:'AI content creation tools can benefit many content creators by saving time and effort, automating tedious tasks, and generating insights. AI Tools that can generate social media posts from blog posts, videos, and other long-form content.'}
  ]

</script>

<div class=" px-5 lg:px-7 pt-[72px] lg:pt-[75px] xl:pt-[50px] pb-[73px] min-h-screen xl:max-h-screen xl:overflow-y-auto flex flex-col xl:pb-[91px] scrollbar-thin scrollbar-track-neutral-800 scrollbar-thumb-neutral-700 ">

  <div class="flex flex-col gap-5">

    <div class="bg-[#343839] rounded-md flex gap-[10px] sm:gap-x-[15px] lg:gap-x-[17px]  py-4 sm:py-5 px-[10px] sm:px-[15px] lg:px-5 lg:py-6">
      <div>
        <img src={profile} alt="profile" class="w-8 h-8 sm:h-10 sm:w-10 lg:h-14 lg:w-14 xl:h-16 xl:w-16 flex-1 rounded-full" />
      </div>

      <div class=" lg:text-base flex flex-col gap-y-2 sm:gap-y-3 lg:gap-y-[14px] xl:gap-y-4">
        <div class="text-neutral-400 font-medium text-[15px] sm:text-base lg:text-[17px] xl:text-[18px]">Prompt type : <span class="text-white font-normal text-sm sm:text-[15px] lg:text-base xl:text-[16.5px]">Introduction</span>
        </div>

        <div class="text-neutral-400 font-medium text-[15px] sm:text-base lg:text-[17px] xl:text-[18px]">Subject : <span class="text-white font-normal text-sm sm:text-[15px] lg:text-base xl:text-[16.5px]">AI helps in UI/UX design</span>
        </div>

        <div class="text-neutral-400 font-medium text-[15px] sm:text-base lg:text-[17px] xl:text-[18px]">Demographics : <span class="text-white font-normal text-sm sm:text-[15px] lg:text-base xl:text-[16.5px]">5 lines</span></div>
      </div>

    </div>

    {#each gptchats as {title,msg} (title)}
      <div class="flex gap-[10px] sm:gap-x-[15px] lg:gap-x-[17px] py-4 sm:py-5 px-[10px] sm:px-[15px]">
        
        <div>
          <img src={gpt} alt="gpt" class="w-8 h-8 sm:h-10 sm:w-10 lg:h-14 lg:w-14 xl:h-16 xl:w-16 flex-1 rounded-full" />
        </div>

        <div class="flex flex-col gap-y-1 sm:gap-y-[7px] xl:gap-y-[9px] text-[15px]  flex-1">
          <div class="text-white font-medium sm:text-base lg:text-[17px] xl:text-[18px]">{title}</div>
          <p class="text-sm text-neutral-400 sm:text-[15px] lg:text-base xl:text-[16.5px] leading-normal sm:leading-relaxed lg:leading-[1.69]">{msg}</p>
        </div>

      </div>
    {/each}

  </div>

  <div class="flex-1 flex items-end justify-end pt-7 pb-[15px] sm:pb-[24px] xl:pb-8 text-neutral-400 font-medium text-xs">Words used : 12000</div>


</div>




