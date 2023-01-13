<script>
  import Header from "../components/Header.svelte";
  import Silderbar from "../components/Siderbar.svelte";
  import Main from "../components/Main.svelte";
  import TimeLine from "../components/TimeLine.svelte";
</script>

<style>
  :global(body){
    background-color: #676778;
    color: white;
  }
</style>

<Header />
<Main>
  <TimeLine />
  <Silderbar />
</Main>