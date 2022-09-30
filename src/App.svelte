<script>
//   import { slide } from 'svelte/types/runtime/transition';
// import svelteLogo from './assets/svelte.svg'
import { onMount } from "svelte";
  import Header from "./components/Header.svelte";
  import Main from "./components/Main.svelte";
  import Sidebar from "./components/Sidebar.svelte"
  import TimeLine from "./components/TimeLine.svelte"; 

  let data = {}
  // const API = "http://localhost:8001/pugstagram";
  const API = "https://kittygram-api.vercel.app/";

  onMount(async () => {
    const response = await fetch(API); 
    data = await response.json();
  })
</script>

<Header />
<Sidebar {...data.user} />
<TimeLine  posts={data.posts} />
<style>
  @import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');
  @import url('https://fonts.googleapis.com/css2?family=Lato&family=Pacifico&display=swap');
  :global(body) {
    background-color: #fafafa;
    color:rgba(38, 38, 38, 0.7);
    font-family: "Lato", sans-serif;
    margin: 0;
    padding: 0;
  }
  :global(h1, h2, h3){
    margin:0;
    padding: 0;
  }
</style>
