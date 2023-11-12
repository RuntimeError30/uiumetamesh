<script>
  import appF from '../Imgs/appf.jpg'
  import sporC from '../Imgs/sportsClub.jpg'
  import Darain from '../Imgs/darain.jpg'
</script>

<div class="text-white flex mt-10 justify-end z-50 col-span-2">
  <div class="mr-10 flex flex-col items-end">
    <div class="border-b-[1px] border-stone-600 pb-4 w-72">
      <h1
        class=" font-light uppercase text-xs flex itemt-start w-full
        rounded-sm transition-all"
      >
        Your Club & Forums
      </h1>
      <ul class="flex flex-col itemt-end mt-2">
        <li class="">
          <a href="" class="flex items-center font-bold uppercase tracking-wider">
            <img src={appF} alt="" class="aspect-square w-10 rounded-xl" />
            <h1 class="ml-2 text-base">UIU App Forum</h1>
          </a>
        </li>

        <li class="mt-3">
          <a href="" class="flex items-center font-bold uppercase tracking-wider">
            <img src={sporC} alt="" class="aspect-square w-10 rounded-xl" />
            <h1 class="ml-2 text-base">UIU Sports Club</h1>
          </a>
        </li>
      </ul>
    </div>

    <div class="w-72 mt-10 border-b border-stone-600 pb-9">
      <h1
        class=" font-light uppercase text-xs flex itemt-start w-full
        rounded-sm transition-all mb-5"
      >
        Upcoming Events
      </h1>
      <ul class="flex flex-col itemt-end mt-2">
        <li class="mt-3">
          <div class="flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-6 h-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 012.25-2.25h13.5A2.25 2.25 0 0121 7.5v11.25m-18 0A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75m-18 0v-7.5A2.25 2.25 0 015.25 9h13.5A2.25 2.25 0 0121 11.25v7.5m-9-6h.008v.008H12v-.008zM12 15h.008v.008H12V15zm0 2.25h.008v.008H12v-.008zM9.75 15h.008v.008H9.75V15zm0 2.25h.008v.008H9.75v-.008zM7.5 15h.008v.008H7.5V15zm0 2.25h.008v.008H7.5v-.008zm6.75-4.5h.008v.008h-.008v-.008zm0 2.25h.008v.008h-.008V15zm0 2.25h.008v.008h-.008v-.008zm2.25-4.5h.008v.008H16.5v-.008zm0 2.25h.008v.008H16.5V15z"
              />
            </svg>

            <h1 class="text-sm uppercase text-stone-500">November 31, 2023</h1>
          </div>
          <h1 class="text-orange-500">UIU Premik Purush Dibosh</h1>
        </li>

        <li class=" mt-2">
          <a href="" class="hover:text-orange-500 flex items-center">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-4 h-4"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M12 9v6m3-3H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
              />
            </svg>

            <h1 class="text-xs ml-1">See More Events</h1>
          </a>
        </li>
      </ul>
    </div>

    <div class="w-72 mt-10">
      <div class="flex items-center justify-between">
        <h1>Active Users</h1>
        <button class="">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
            />
          </svg>
        </button>
      </div>

      <div class="mt-5 h-[23rem] overflow-y-scroll" id="activeU">
        <a href="" class="flex items-center mb-5">
          <img src={Darain} alt="" class="aspect-square object-cover w-10 rounded-full" />

          <div class="flex items-center justify-between w-full">
            <h1 class="ml-2">Mohammad Darain Khan</h1>

            <div class="w-3 h-3 bg-lime-500 rounded-full aspect-square" />
          </div>
        </a>

        <a href="" class="flex items-center mb-5">
          <img src={Darain} alt="" class="aspect-square object-cover w-10 rounded-full" />

          <div class="flex items-center justify-between w-full">
            <h1 class="ml-2">Abaro Mohammad Darain Khan</h1>

            <div class="w-3 h-3 bg-lime-500 rounded-full aspect-square" />
          </div>
        </a>

        <a href="" class="flex items-center mb-5">
          <img src={Darain} alt="" class="aspect-square object-cover w-10 rounded-full" />

          <div class="flex items-center justify-between w-full">
            <h1 class="ml-2">Abaro Abaro Mohammad Darain Khan</h1>

            <div class="w-3 h-3 bg-lime-500 rounded-full aspect-square" />
          </div>
        </a>

        <a href="" class="flex items-center mb-5">
          <img src={Darain} alt="" class="aspect-square object-cover w-10 rounded-full" />

          <div class="flex items-center justify-between w-full">
            <h1 class="ml-2">Abaro Abaro Abaro Mohammad Darain Khan</h1>

            <div class="w-3 h-3 bg-lime-500 rounded-full aspect-square" />
          </div>
        </a>
      </div>
    </div>
  </div>
</div>
