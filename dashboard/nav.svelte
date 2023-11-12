<script>
  import logo from '../Imgs/logo.png'
  import Darain from '../Imgs/darain.jpg'
</script>

<nav
  class="sticky top-0 left-0 right-0 bg-opacity-60 flex justify-between bg-stone-950 border-r rounded-r-xl border-orange-500"
>
  <div class="flex w-fit p-5">
    <a href="/" class=""><img src={logo} alt="UIU METAMESH" class="w-48 ml-5" /></a>

    <div class="p-4 flex text-white">
      <input
        type="text"
        name=""
        id=""
        placeholder="Search"
        class="placeholder:text-xs bg-stone-900 p-1 w-80 rounded-lg outline-none shadow-inner ml-10"
      />

      <button>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-7 h-7 text-orange-500 relative right-7
                "
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M15.75 15.75l-2.489-2.489m0 0a3.375 3.375 0 10-4.773-4.773 3.375 3.375 0 004.774 4.774zM21 12a9 9 0 "
          />
        </svg>
      </button>
    </div>
  </div>

  <ul class="flex items-center space-x-5 mr-10 text-white">
    <li>
      <a href="">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="currentColor"
          class="w-8 h-8 text-orange-500"
        >
          <path
            fill-rule="evenodd"
            d="M5.25 9a6.75 6.75 0 0113.5 0v.75c0 2.123.8 4.057 2.118 5.52a.75.75 0 01-.297 1.206c-1.544.57-3.16.99-4.831 1.243a3.75 3.75 0 11-7.48 0 24.585 24.585 0 01-4.831-1.244.75.75 0 01-.298-1.205A8.217 8.217 0 005.25 9.75V9zm4.502 8.9a2.25 2.25 0 104.496 0 25.057 25.057 0 01-4.496 0z"
            clip-rule="evenodd"
          />
        </svg>
      </a>
    </li>
    <li class="">
      <a href="">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="currentColor"
          class="w-8 h-8 text-orange-500"
        >
          <path
            fill-rule="evenodd"
            d="M5.337 21.718a6.707 6.707 0 01-.533-.074.75.75 0 01-.44-1.223 3.73 3.73 0 00.814-1.686c.023-.115-.022-.317-.254-.543C3.274 16.587 2.25 14.41 2.25 12c0-5.03 4.428-9 9.75-9s9.75 3.97 9.75 9c0 5.03-4.428 9-9.75 9-.833 0-1.643-.097-2.417-.279a6.721 6.721 0 01-4.246.997z"
            clip-rule="evenodd"
          />
        </svg>
      </a>
    </li>
    <li class="mr-16 flex">
      <a href="" class="">
        <img src={Darain} alt="" class="aspect-square w-10 rounded-full object-cover" />
      </a>
    </li>
  </ul>
</nav>
