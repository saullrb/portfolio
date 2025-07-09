<template>
  <header id="navbar" class="fixed w-full">
    <div class="navbar bg-base-300 shadow-sm">
      <div class="navbar-start">
        <a href="#" class="btn btn-ghost text-xl">Home</a>
      </div>
      <div class="navbar-end">
        <ul class="menu menu-horizontal px-1 hidden sm:flex">
          <li><a href="#projects">Projects</a></li>
          <li><a href="#skills">Skills</a></li>
        </ul>
        <div class="dropdown dropdown-end">
          <div tabindex="0" role="button" class="btn btn-ghost sm:hidden">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h8m-8 6h16"
              />
            </svg>
          </div>
          <ul
            tabindex="0"
            class="menu dropdown-content bg-base-200 rounded-box z-1 mt-3 w-52 p-2 shadow"
          >
            <li><a href="#projects">Projects</a></li>
            <li><a href="#skills">Skills</a></li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>
