<script>
  import Darain from '../Imgs/darain.jpg';
  import Taseen from '../Imgs/Taseen.jpg';
  import Dip from '../Imgs/dip.jpg';
  import { gsap } from "gsap";
  import { onMount } from 'svelte'

  let turnOn = false
  function openTab() {
    turnOn = !turnOn
  }

  function closeTab() {
    turnOn = false;
  }


  let onComments = false;
  function comments(){
    onComments = !onComments;
  }






</script>

<section class="col-span-8 grid h-[54rem] justify-center text-white overflow-auto">
  <div class="w-full mt-5">
    <div class="flex flex-col bg-stone-950 rounded-xl w-[70rem] p-5">
      <label for="" class=" uppercase text-xs mb-4">Darain, Post Something to your friends </label>
      <input
        type="text"
        class="h-16 rounded-xl border bg-stone-900 border-orange-500"
        on:click={openTab}
      />

      <div class="flex items-center w-full mt-3">
        <button
          class="flex border border-stone-600 hover:border-orange-500 transition-all ease-in- items-center p-3 w-full mr-3 rounded-xl"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-5 h-5 text-red-500"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M6.827 6.175A2.31 2.31 0 015.186 7.23c-.38.054-.757.112-1.134.175C2.999 7.58 2.25 8.507 2.25 9.574V18a2.25 2.25 0 002.25 2.25h15A2.25 2.25 0 0021.75 18V9.574c0-1.067-.75-1.994-1.802-2.169a47.865 47.865 0 00-1.134-.175 2.31 2.31 0 01-1.64-1.055l-.822-1.316a2.192 2.192 0 00-1.736-1.039 48.774 48.774 0 00-5.232 0 2.192 2.192 0 00-1.736 1.039l-.821 1.316z"
            />
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M16.5 12.75a4.5 4.5 0 11-9 0 4.5 4.5 0 019 0zM18.75 10.5h.008v.008h-.008V10.5z"
            />
          </svg>
          <h1>Upload Photos</h1>
        </button>

        <div class="w-full">
          <select
            name=""
            id=""
            class="bg-transparent border rounded-xl w-full p-3 border-stone-600"
          >
            <option value="Urgent" class="text-black">Urgent</option>
            <option value="Urgent" class="text-black">Regular</option>
            <option value="Urgent" class="text-black">Question</option>
            <option value="Urgent" class="text-black">Help</option>
          </select>
        </div>
      </div>
    </div>

    <!-- POP UP UPLOAD BOX -->

    {#if turnOn}
      <div class="w-[70rem] flex justify-center fixed">
        <div class="p-5 w-fit rounded-xl bg-stone-950">
          <div class="flex items-center justify-between mb-4">
            <div class="flex items-center">
              <img src={Darain} alt="" class="aspect-square w-10 rounded-full object-cover" />

              <h1 class="text-lg font-semibold ml-2">Mohammad Darain Khan</h1>
            </div>

            <button class="hover:text-orange-500" on:click={closeTab}>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-6 h-6"
              >
                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
              </svg>
            </button>
          </div>

          <div />

          <div class="flex flex-col">
            <textarea
              name=""
              id=""
              cols="50"
              rows="10"
              class="resize-none rounded-xl border bg-stone-900 outline-none border-orange-500 p-5"
              placeholder="Post Something"
            />
            <div class="flex items-center w-full mt-3">
              <button
                class="flex hover:border-orange-500 transition-all ease-in- items-center border p-3 w-full mr-3 rounded-xl"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-5 h-5 text-red-500"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M6.827 6.175A2.31 2.31 0 015.186 7.23c-.38.054-.757.112-1.134.175C2.999 7.58 2.25 8.507 2.25 9.574V18a2.25 2.25 0 002.25 2.25h15A2.25 2.25 0 0021.75 18V9.574c0-1.067-.75-1.994-1.802-2.169a47.865 47.865 0 00-1.134-.175 2.31 2.31 0 01-1.64-1.055l-.822-1.316a2.192 2.192 0 00-1.736-1.039 48.774 48.774 0 00-5.232 0 2.192 2.192 0 00-1.736 1.039l-.821 1.316z"
                  />
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M16.5 12.75a4.5 4.5 0 11-9 0 4.5 4.5 0 019 0zM18.75 10.5h.008v.008h-.008V10.5z"
                  />
                </svg>
                <h1>Upload Photos</h1>
              </button>

              <div class="w-full">
                <select name="" id="" class="bg-transparent border rounded-xl w-full p-3">
                  <option value="Urgent" class="text-black">Urgent</option>
                  <option value="Urgent" class="text-black">Regular</option>
                  <option value="Urgent" class="text-black">Question</option>
                  <option value="Urgent" class="text-black">Help</option>
                </select>
              </div>
            </div>
            <button
              class="w-full rounded-lg p-2 mt-5 bg-orange-600 uppercase hover:bg-orange-500 transition-all ease-in"
              >Post</button
            >
          </div>
        </div>
      </div>
    {/if}

    <!-- Pop up upload box area finishes here -->

    <div class="mt-5 flex flex-col bg-stone-950 rounded-xl w-[70rem] p-5">
      <a href="" class="flex items-center">
        <img src={Darain} alt="" class="aspect-square w-8 rounded-full object-cover" />

        <h1 class="text-sm font-base ml-2">Mohammad Darain Khan</h1>
      </a>

      <h1 class="text-lg mt-5">Ai fun mari React er! Svelte bosss</h1>

      <div class="flex items-center mt-5">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-4 h-4 text-orange-500"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M6.633 10.5c.806 0 1.533-.446 2.031-1.08a9.041 9.041 0 012.861-2.4c.723-.384 1.35-.956 1.653-1.715a4.498 4.498 0 00.322-1.672V3a.75.75 0 01.75-.75A2.25 2.25 0 0116.5 4.5c0 1.152-.26 2.243-.723 3.218-.266.558.107 1.282.725 1.282h3.126c1.026 0 1.945.694 2.054 1.715.045.422.068.85.068 1.285a11.95 11.95 0 01-2.649 7.521c-.388.482-.987.729-1.605.729H13.48c-.483 0-.964-.078-1.423-.23l-3.114-1.04a4.501 4.501 0 00-1.423-.23H5.904M14.25 9h2.25M5.904 18.75c.083.205.173.405.27.602.197.4-.078.898-.523.898h-.908c-.889 0-1.713-.518-1.972-1.368a12 12 0 01-.521-3.507c0-1.553.295-3.036.831-4.398C3.387 10.203 4.167 9.75 5 9.75h1.053c.472 0 .745.556.5.96a8.958 8.958 0 00-1.302 4.665c0 1.194.232 2.333.654 3.375z"
          />
        </svg>

        <h1 class="ml-1">69</h1>
      </div>

      <div class="flex mt-5 space-x-7">
        <button
          class="border border-stone-600 hover:bg-orange-500 p-2 rounded-xl w-1/2 flex justify-center"
        >
          <!-- svelte-ignore a11y-click-events-have-key-events -->
          <!-- svelte-ignore a11y-no-static-element-interactions -->
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
            on:click={bgColor}
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M6.633 10.5c.806 0 1.533-.446 2.031-1.08a9.041 9.041 0 012.861-2.4c.723-.384 1.35-.956 1.653-1.715a4.498 4.498 0 00.322-1.672V3a.75.75 0 01.75-.75A2.25 2.25 0 0116.5 4.5c0 1.152-.26 2.243-.723 3.218-.266.558.107 1.282.725 1.282h3.126c1.026 0 1.945.694 2.054 1.715.045.422.068.85.068 1.285a11.95 11.95 0 01-2.649 7.521c-.388.482-.987.729-1.605.729H13.48c-.483 0-.964-.078-1.423-.23l-3.114-1.04a4.501 4.501 0 00-1.423-.23H5.904M14.25 9h2.25M5.904 18.75c.083.205.173.405.27.602.197.4-.078.898-.523.898h-.908c-.889 0-1.713-.518-1.972-1.368a12 12 0 01-.521-3.507c0-1.553.295-3.036.831-4.398C3.387 10.203 4.167 9.75 5 9.75h1.053c.472 0 .745.556.5.96a8.958 8.958 0 00-1.302 4.665c0 1.194.232 2.333.654 3.375z"
            />
          </svg>
        </button>

        <button
          class="border border-stone-600 hover:bg-orange-500 p-2 rounded-xl w-1/2 flex justify-center"
          on:click={comments}
        >
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
              d="M8.625 12a.375.375 0 11-.75 0 .375.375 0 01.75 0zm0 0H8.25m4.125 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zm0 0H12m4.125 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zm0 0h-.375M21 12c0 4.556-4.03 8.25-9 8.25a9.764 9.764 0 01-2.555-.337A5.972 5.972 0 015.41 20.97a5.969 5.969 0 01-.474-.065 4.48 4.48 0 00.978-2.025c.09-.457-.133-.901-.467-1.226C3.93 16.178 3 14.189 3 12c0-4.556 4.03-8.25 9-8.25s9 3.694 9 8.25z"
            />
          </svg>
        </button>
      </div>

      {#if onComments}
        <div class="mt-5 space-y-5">
          <div class="bg-stone-900 p-3 rounded-xl">
            <div>
              <a href="" class="flex items-center">
                <img src={Darain} alt="" class="aspect-square w-8 rounded-full object-cover" />

                <h1 class="text-sm font-base ml-2">Mohammad Darain Khan</h1>
              </a>
            </div>
            <div>
              <h1 class="ml-10">e bodda e boddaaa</h1>
            </div>
          </div>
        </div>
      {/if}
    </div>

    <div class="mt-5 flex flex-col bg-stone-950 rounded-xl w-[70rem] p-5">
      <a href="" class="flex items-center">
        <img src={Taseen} alt="" class="aspect-square w-8 rounded-full object-cover" />

        <h1 class="text-sm font-base ml-2">Taseen Chowdhury</h1>
      </a>

      <h1 class="text-lg mt-5">Dip De Jango Pare</h1>

      <div class="flex items-center mt-5">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-4 h-4 text-orange-500"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M6.633 10.5c.806 0 1.533-.446 2.031-1.08a9.041 9.041 0 012.861-2.4c.723-.384 1.35-.956 1.653-1.715a4.498 4.498 0 00.322-1.672V3a.75.75 0 01.75-.75A2.25 2.25 0 0116.5 4.5c0 1.152-.26 2.243-.723 3.218-.266.558.107 1.282.725 1.282h3.126c1.026 0 1.945.694 2.054 1.715.045.422.068.85.068 1.285a11.95 11.95 0 01-2.649 7.521c-.388.482-.987.729-1.605.729H13.48c-.483 0-.964-.078-1.423-.23l-3.114-1.04a4.501 4.501 0 00-1.423-.23H5.904M14.25 9h2.25M5.904 18.75c.083.205.173.405.27.602.197.4-.078.898-.523.898h-.908c-.889 0-1.713-.518-1.972-1.368a12 12 0 01-.521-3.507c0-1.553.295-3.036.831-4.398C3.387 10.203 4.167 9.75 5 9.75h1.053c.472 0 .745.556.5.96a8.958 8.958 0 00-1.302 4.665c0 1.194.232 2.333.654 3.375z"
          />
        </svg>

        <h1 class="ml-1">1</h1>
      </div>

      <div class="flex mt-5 space-x-7">
        <button
          class="border border-stone-600 hover:bg-orange-500 p-2 rounded-xl w-1/2 flex justify-center"
        >
          <!-- svelte-ignore a11y-click-events-have-key-events -->
          <!-- svelte-ignore a11y-no-static-element-interactions -->
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
            on:click={bgColor}
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M6.633 10.5c.806 0 1.533-.446 2.031-1.08a9.041 9.041 0 012.861-2.4c.723-.384 1.35-.956 1.653-1.715a4.498 4.498 0 00.322-1.672V3a.75.75 0 01.75-.75A2.25 2.25 0 0116.5 4.5c0 1.152-.26 2.243-.723 3.218-.266.558.107 1.282.725 1.282h3.126c1.026 0 1.945.694 2.054 1.715.045.422.068.85.068 1.285a11.95 11.95 0 01-2.649 7.521c-.388.482-.987.729-1.605.729H13.48c-.483 0-.964-.078-1.423-.23l-3.114-1.04a4.501 4.501 0 00-1.423-.23H5.904M14.25 9h2.25M5.904 18.75c.083.205.173.405.27.602.197.4-.078.898-.523.898h-.908c-.889 0-1.713-.518-1.972-1.368a12 12 0 01-.521-3.507c0-1.553.295-3.036.831-4.398C3.387 10.203 4.167 9.75 5 9.75h1.053c.472 0 .745.556.5.96a8.958 8.958 0 00-1.302 4.665c0 1.194.232 2.333.654 3.375z"
            />
          </svg>
        </button>

        <button
          class="border border-stone-600 hover:bg-orange-500 p-2 rounded-xl w-1/2 flex justify-center"
          on:click={comments}
        >
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
              d="M8.625 12a.375.375 0 11-.75 0 .375.375 0 01.75 0zm0 0H8.25m4.125 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zm0 0H12m4.125 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zm0 0h-.375M21 12c0 4.556-4.03 8.25-9 8.25a9.764 9.764 0 01-2.555-.337A5.972 5.972 0 015.41 20.97a5.969 5.969 0 01-.474-.065 4.48 4.48 0 00.978-2.025c.09-.457-.133-.901-.467-1.226C3.93 16.178 3 14.189 3 12c0-4.556 4.03-8.25 9-8.25s9 3.694 9 8.25z"
            />
          </svg>
        </button>
      </div>

      <div class="mt-5 space-y-5">
        <div class="bg-stone-900 p-3 rounded-xl">
          <div>
            <a href="" class="flex items-center">
              <img src={Darain} alt="" class="aspect-square w-8 rounded-full object-cover" />

              <h1 class="text-sm font-base ml-2">Mohammad Darain Khan</h1>
            </a>
          </div>
          <div>
            <h1 class="ml-10">Amio Donald Trump</h1>
          </div>
        </div>

        <div class="bg-stone-900 p-3 rounded-xl">
          <div>
            <a href="" class="flex items-center">
              <img src={Dip} alt="" class="aspect-square w-8 rounded-full object-cover" />

              <h1 class="text-sm font-base ml-2">Dip Saha</h1>
            </a>
          </div>
          <div>
            <h1 class="ml-10">To Ai kittam?</h1>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
