<template>
  <nav class="fixed z-10 w-full flex items-center bg-white">
    <div class="nav__links mr-auto text-xl">
      <a href="#contact">تواصل معنا</a> |
      <router-link to="/">الرئيسية</router-link>
    </div>
    <div class="logo mr-auto">
      <a href="/">
        <img class="w- h-10" src="./assets/images/logo.png" alt=""
      /></a>
    </div>
  </nav>

  <router-view />
  <footer class="text-gray-700 p-3 mx-1 mb-1" id="contact">
    <div class="info__container mb-10 bg-yellow-100 p-5 rounded-2xl">
      <h2 class="text-gray-700 text-3xl font-bold mr-7 mb-5">تواصل معنا</h2>
      <div class="info my-16 flex flex-col lg:flex lg:flex-row">
        <span
          class="flex flex-col lg:flex lg:flex-row lg:items-center md:flex md:flex-row md:items-center my-10 mail text-gray-700 text-2xl font-bold mr-7"
          >إيميل:
          <a
            class="bg-gray-700 text-xl mt-5 my-3 text-center max-w-xs text-white rounded-xl p-2 mx-3 hover:text-white hover:bg-slate-500"
            href="mailto:aboomar6961@yahoo.com"
            >aboomar6961@yahoo.com</a
          ></span
        >
        <span
          class="flex flex-col lg:flex lg:flex-row lg:items-center md:flex md:flex-row md:items-center my-10 phone text-gray-700 text-2xl font-bold mr-7"
          >موبايل:
          <a
            class="bg-gray-700 text-xl text-center my-3 max-w-xs text-white rounded-xl p-2 mx-6 hover:text-white hover:bg-slate-500"
            href="tel:+201001098112"
            >201001098112+</a
          >
          <a
            class="bg-gray-700 text-xl text-center my-3 max-w-xs text-white rounded-xl p-2 mx-6 hover:text-white hover:bg-slate-500"
            href="tel:+201007995990"
            >201007995990+</a
          ></span
        >
      </div>
    </div>
    <p class="mt-10 text-center">Copyright © 2023 Yusuf - Development.</p>
  </footer>
</template>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: cairo;
  transition: 0.6 ease !important;
}

html {
  scroll-behavior: smooth;
}

nav {
  padding: 30px;
  transition: 0.6 ease;
  a {
    font-weight: bold;
    color: #2c3e50;
    transition: 0.6 ease;
    &.router-link-exact-active {
      color: #946508;
    }
  }
}

section {
  p,
  li {
    font-weight: bold;
    color: #2c3e50;
    transition: 0.6 ease;
  }
}

a:hover {
  transition: 0.6s ease;
  color: #553c09;
}
</style>
