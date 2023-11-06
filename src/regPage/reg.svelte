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
   
        setTimeout(() => {goto('/');}, 300);
    

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


<div class=" h-full w-full">
    <div class="flex  justify-end">
        <div class=" bg-white  p-3 rounded-l-xl">        
            <h1 class=" tracking-wider text-right text-4xl font-black "style="font-family: 'Playfair Display', serif;">Sign Up</h1>
            <h1 class=" text-xs uppercase mt-1">with your University credentials to join metamesh community</h1></div>

    </div>


    <form action="" class="w-full h-fit grid ">
        <div class="w-full h-fit  mt-20 flex flex-wrap justify-center ">
            <div class="bg-white grid  w-fit p-10 rounded-xl ml-20">


                <div class="grid mb-10 mt-5 ">
                    <input type="text" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class=" uppercase h-fit justify-center ">First Name</span>
                </div>
    
                <div class="grid mb-10">
                    <input type="text" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">Last Name</span>
                </div>
    
                <div class="grid mb-10">
                    <input type="text" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">university Email</span>
                </div>
    
                <div class="grid mb-10">
                    <input type="text" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">Student ID</span>
                </div>
    
    
                <div class="grid  ">
                    <input type="Password" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">batch</span>
                </div>
            </div>
    
    
    
    
    
    
    
    
    
            <div class="bg-white grid  w-fit p-10 rounded-xl ml-20">
    
    
                <div class="grid mb-10 mt-5">
                    <input type="Password" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">New Password</span>
                </div>
    
                <div class="grid mb-10">
                    <input type="Password" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">Re-Type New Password</span>
                </div>
    
                <div class="grid mb-10">
                    <input type="text" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">Mobile Number</span>
                </div>
    
                <div class="grid ">
                    <input type="Password" id="passwordInput" class="inpbox border-b border-black w-[40vh] outline-none placeholder:text-xs" onclick="upd()" required="required">
                    <span for="" id="mailLab" class="text-sm  uppercase h-fit justify-center ">Department</span>
                </div>
            </div>
        </div>

        <button class="flex justify-center mt-5 w-full">
            <div class=" flex justify-center border rounded-full ml-20 bg-white">
                <!-- svelte-ignore a11y-no-static-element-interactions -->
                <div class="h-16 w-16 rounded-full border  " style="background-color: {isMouseEnter ? "black" : "transparent"};
                transition: background-color 0.3s ease;" on:mouseenter={handleMouseEnter} on:mouseleave={handleMouseLeave}>
                    

                    <svg xmlns="http://www.w3.org/2000/svg" id="circleInnerArrow" class=" relative  top-5 text-white left-5 h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M17 8l4 4m0 0l-4 4m4-4H3" />
                      </svg>
                </div>

             
                <span class="relative right-5  top-5" style="margin-left: {isMouseEnter ? "25px" : "0"};
                transition: margin-left 0.3s ease;">Sign Up!</span>
            </div>

        </button>





    </form>

    <div class=" w-full  ">
        <a href="/" class="text-xs h-fit ml-20 flex justify-center text-white relative  top-4 uppercase">I Already have an account</a>
    </div>
    

</div>