<script>
  import { onMount } from "svelte";
  import Header from "../components/Header.svelte";
  import Main from "../components/Main.svelte";
  import TimeLine from "../components/TimeLine.svelte";
  import Siderbar from "../components/Siderbar.svelte";

  let data = {};
  const API ="https://kittygram-api.vercel.app/";
  onMount(async () => {
    const response = await fetch(API);
    data = await response.json();
  });
</script>

<Header />
<Main>
  <TimeLine posts={data.posts}/>
  <Siderbar {...data.user}/>
</Main>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Lato:wght@300");
  @import url("https://fonts.googleapis.com/css2?family=Pacifico&display=swap");
  :global(body) {
    margin: 0;
    padding: 0;
    background-color: #fafafa;
    color: rgba(38, 38, 38, 0.7);
    font-family: "Lato", sans-serif;
  }
</style>
