
<script lang="ts">
  import Header from "../components/Header.svelte"
  import Chat from "../components/Chat.svelte"
  import Input from "../components/Input.svelte"
  import DeskMenu from "../components/DeskMenu.svelte";
  import DeskHistory from "../components/DeskHistory.svelte";
</script>


<div class="xl:hidden">

  <Header />

  <Chat />

  <Input />

</div>

<div class="hidden xl:flex h-screen ">

  <DeskMenu />

  <div class="flex-1 relative  ">
    <Chat />
    <Input />
  </div>

  <DeskHistory />

</div>

