<script>
    import { goto } from '$app/navigation';
    import BGvid from '../Vids/bgVid.mp4';
    let isMouseEnter = false;

    function handleMouseEnter(){
        isMouseEnter = true;
    }

    function handleMouseLeave(){
        isMouseEnter = false;
    }



    function handleScroll(event) {
        setTimeout(() => {goto('/registration');}, 300);
    

  }



    
</script>

<style>
    .input-container span{
        transition: 0.5s;
    }
    .input-container input:valid ~ span,
    .input-container input:focus ~ span{
        transform: translateY(-20px);
        font-size: 12px;

    }


    button {
    transition: padding 0.2s; /* Add a transition for smooth animation */
}

.button-hovered {
    padding-left: 30px; /* Adjust the padding as needed */
}








</style>



<svelte:window on:wheel={handleScroll} />
<section class="h-full w-full flex justify-end">
    <div class="text-white bg-gradient-to-l from-stone-950 via-stone-950 to-transparent h-[50vh] mt-16 w-fit">

        <div class="w-fit flex realtive ">      
              

            <h1 style="font-family: 'Playfair Display', serif;  -webkit-text-fill-color: transparent; 
            -webkit-text-stroke: 1px white; 
            writing-mode: vertical-lr;
            " class="text-7xl relative left-4 opacity-5 font-black">UIU Metamesh</h1>


            <h1 style="font-family: 'Playfair Display', serif;  -webkit-text-fill-color: transparent; 
            -webkit-text-stroke: 1px white; 
            writing-mode: vertical-lr;
            " class="text-7xl font-black opacity-20">UIU Metamesh</h1>
            
            <h1 style="font-family: 'Playfair Display', serif;  -webkit-text-fill-color: transparent; 
            -webkit-text-stroke: 1px white; 
            writing-mode: vertical-lr;
            " class="text-7xl relative right-4 opacity-50 font-black">UIU Metamesh</h1>

            <h1 style="font-family: 'Playfair Display', serif;  -webkit-text-fill-color: transparent; 
            -webkit-text-stroke: 1px white; 
            writing-mode: vertical-lr;
            " class="text-7xl relative right-9 opacity-70 font-black">UIU Metamesh</h1>

            <h1 style="font-family: 'Playfair Display', serif;  
            writing-mode: vertical-lr;
            " class="text-7xl relative right-14 opacity-100 font-black">UIU Metamesh</h1>
        </div>
    </div>




    <div class="h-full flex justify-end ">
        <form action="" class=" grid justify-center  rounded-l-3xl  bg-white p-10  w-fit backdrop-blur-3xl ">
            <div class="mt-20">

                <div class="relative bottom-12 mb-20">
           
                    <h1 class=" text-5xl tracking-wide font-bold uppercase " style="font-family: 'Playfair Display', serif;">Login</h1>
                    <h1 class="text-xs uppercase">to continue to your metaverse profile</h1>
                </div>
                <div class="input-container grid">
    
                    <input type="text" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm absolute h-fit justify-center ">STUDENT ID OR EMAIL</span>
                </div>
    
    
                <div class="input-container grid mt-16">
    
                    <input type="Password" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm absolute uppercase h-fit justify-center ">Password</span>
                   

                </div>

                
                <a href="" class="text-xs relative bottom-20">I'VE LOST MY PASSWORD</a>


                <button >
                    <div class="flex justify-center mt-10 ">
                        <!-- svelte-ignore a11y-no-static-element-interactions -->
                        <div class="h-16 w-16 rounded-full border border-slate-300 " style="background-color: {isMouseEnter ? "black" : "transparent"};
                        transition: background-color 0.3s ease;" on:mouseenter={handleMouseEnter} on:mouseleave={handleMouseLeave}>
                            

                            <svg xmlns="http://www.w3.org/2000/svg" id="circleInnerArrow" class=" relative  top-5 text-white left-5 h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M17 8l4 4m0 0l-4 4m4-4H3" />
                              </svg>
                        </div>

                     
                        <span class="relative right-5  top-5" style="margin-left: {isMouseEnter ? "25px" : "0"};
                        transition: margin-left 0.3s ease;">Login</span>
                    </div>

                </button>


                <div class="w-full h-fit mt-12 uppercase text-xs animate-pulse">
                    <span class="flex justify-center"> <a href="/registration">Click here or scroll down if you are new here</a> </span>
                </div>
            
    
            </div>
        </form>
    </div>



</section>