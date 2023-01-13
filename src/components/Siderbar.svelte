<script>
  import Profile from "./Profile.svelte";
  import Stories from "./Stories.svelte";
  import Footer from "./Footer.svelte";

  export let nickname;
  export let name;
</script>

<div class="Silderbar">
  <div class="Silderbar-container">
    <Profile {nickname} {name}/>
    <Stories />
    <Footer />
  </div>
</div>

<style>
  .Silderbar {
    position: relative;
    padding: 4.5em 0 0 0;
  }
  .Silderbar-container {
    position: fixed;
  }
</style>
