<template>
<nav class="bg-white border-gray-200 dark:bg-gray-900">
  <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
  <a href="https://flowbite.com/" class="flex items-center">
      <img src="https://flowbite.com/docs/images/logo.svg" class="h-8 mr-3" alt="Flowbite Logo" />
      <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">vinn</span>
  </a>
  <div class="flex items-center md:order-2">
      <button type="button" class="flex mr-3 text-sm bg-gray-800 rounded-full md:mr-0 focus:ring-4 focus:ring-gray-300 dark:focus:ring-gray-600" id="user-menu-button" aria-expanded="false" data-dropdown-toggle="user-dropdown" data-dropdown-placement="bottom">
        <span class="sr-only">Open user menu</span>
        <img class="w-8 h-8 rounded-full" src="data:image/jpeg;base64,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" alt="user photo">
      </button>
      <!-- Dropdown menu -->
      <div class="z-50 hidden my-4 text-base list-none bg-white divide-y divide-gray-100 rounded-lg shadow dark:bg-gray-700 dark:divide-gray-600" id="user-dropdown">
        <div class="px-4 py-3">
          <span class="block text-sm text-gray-900 dark:text-white">Bonnie Green</span>
          <span class="block text-sm  text-gray-500 truncate dark:text-gray-400">name@flowbite.com</span>
        </div>
        <ul class="py-2" aria-labelledby="user-menu-button">
          <li>
            <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Dashboard</a>
          </li>
          <li>
            <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Settings</a>
          </li>
          <li>
            <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Earnings</a>
          </li>
          <li>
            <a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Sign out</a>
          </li>
        </ul>
      </div>
      <button data-collapse-toggle="navbar-user" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-user" aria-expanded="false">
        <span class="sr-only">Open main menu</span>
        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
        </svg>
    </button>
  </div>
  <div class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1" id="navbar-user">
    <ul class="flex flex-col font-medium p-4 md:p-0 mt-4 border border-gray-100 rounded-lg bg-gray-50 md:flex-row md:space-x-8 md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
      <li>
        <a href="#" class="block py-2 pl-3 pr-4 text-white bg-blue-700 rounded md:bg-transparent md:text-blue-700 md:p-0 md:dark:text-blue-500" aria-current="page">Home</a>
      </li>
      <li>
        <a href="#" class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">About</a>
      </li>
      <li>
        <a href="#" class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Services</a>
      </li>
      <li>
        <a href="#" class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Pricing</a>
      </li>
      <li>
        <a href="#" class="block py-2 pl-3 pr-4 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Contact</a>
      </li>
    </ul>
  </div>
  </div>
</nav>

</template>