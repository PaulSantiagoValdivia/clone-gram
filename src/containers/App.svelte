<script>
  import Header from "../components/Header.svelte";
  import Main from "../components/Main.svelte";
  import TimeLine from "../components/TimeLine.svelte";
  import Siderbar from "../components/Siderbar.svelte";
</script>

<Header />
<Main>
  <TimeLine />
  <Siderbar />
</Main>

<style>
  :global(body) {
    background-color: #676778;
    color: white;
  }
</style>
