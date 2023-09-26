<template>
  <!-- <nav class="bg-white border-gray-200 dark:bg-gray-900">
    <div
      class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4"
    >
      <a href="https://flowbite.com/" class="flex items-center">
        <img src="@/assets/logo.png" class="h-8 mr-3" alt="Flowbite Logo" />
        <span
          class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
          >WiseMind</span
        >
      </a>
      <button
        data-collapse-toggle="navbar-default"
        type="button"
        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
        aria-controls="navbar-default"
        aria-expanded="false"
      >
        <span class="sr-only">Open main menu</span>
        <svg
          class="w-5 h-5"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 17 14"
        >
          <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M1 1h15M1 7h15M1 13h15"
          />
        </svg>
      </button>
      <div class="hidden w-full md:block md:w-auto" id="navbar-default">
        <ul
          class="font-medium flex flex-col p-4 md:p-0 mt-4 border border-gray-100 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700"
        >
          <li>
            <a
              href="#"
              class="block py-2 pl-3 pr-4 text-white bg-blue-700 rounded md:bg-transparent md:text-blue-700 md:p-0 dark:text-white md:dark:text-blue-500"
              aria-current="page"
              >Home</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent"
              >Study Abroad</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent"
              >Services</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent"
              >About us</a
            >
          </li>
          <li>
            <a
              href="#"
              class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent"
              >Contact</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav> -->

  <nav class="bg-[#fabd49] border-gray-200 dark:bg-gray-900">
    <div
      class="flex flex-wrap justify-between items-center mx-auto max-w-screen-xl p-4"
    >
      <a href="https://flowbite.com" class="flex items-center">
        <img src="@/assets/logo.png" class="h-12 mr-3" alt="Flowbite Logo" />

        <div
          class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
        >
          WiseMind
          <p class="text-sm createBlock">Unlocking Brilliance</p>
        </div>
      </a>
      <div class="flex justify-center text-xl mt-2 font-victor">
        <span> Study in&nbsp;</span>
        <VueWriter
          :array="countries"
          :eraseSpeed="50"
          :typeSpeed="100"
          caret="cursor"
        />
      </div>
    </div>
    <!-- <div class="flex items-center justify-end">
      <a
        href="tel:5541251234"
        class="mr-6 text-sm text-gray-500 dark:text-white hover:underline"
        >(555) 412-1234</a
      >
      <a
        href="#"
        class="text-sm text-blue-600 dark:text-blue-500 hover:underline"
        >contact@wisemind.com</a
      >
    </div> -->
  </nav>
  <nav class="bg-gray-200 text-white dark:bg-gray-700 overflow-scroll">
    <div class="max-w-screen-xl px-4 py-3 mx-auto">
      <div class="flex items-center">
        <ul class="flex flex-row font-medium mt-0 mr-6 space-x-8 text-sm">
          <li>
            <a
              href="#"
              class="text-gray-900 dark:text-white hover:underline"
              aria-current="page"
              >Home</a
            >
          </li>
          <li>
            <a href="#" class="text-gray-900 dark:text-white hover:underline"
              >Services</a
            >
          </li>
          <li>
            <a href="#" class="text-gray-900 dark:text-white hover:underline"
              >Universities</a
            >
          </li>
          <li>
            <a href="#" class="text-gray-900 dark:text-white hover:underline"
              >About Us</a
            >
          </li>
          <li>
            <a href="#" class="text-gray-900 dark:text-white hover:underline"
              >Contact</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
<script setup>
import VueWriter from "vue-writer";
const countries = ["Australia ", "New Zealand ", "USA ", "Canada"];
</script>
<style></style>
