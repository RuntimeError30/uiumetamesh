<script>
	import { fade } from "svelte/transition";
    import "../app.css";
	  import Loginbg from "../loginPage/loginbg.svelte";



    export let data;
    $:({pathname} = data);
  </script>




  



  {#key pathname}

    <div in:fade={{duration:1000}}>
      <Loginbg/>
            
        


        <slot />
    </div>
    
{/key}