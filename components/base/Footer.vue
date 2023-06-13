<template>
  <footer class="max-w-screen-xl px-8 mx-auto">
    <div class="w-full border-y border-[#DDDDDD]">
      <div class="grid xl:grid-cols-4 lg:grid-cols-2 md:grid-cols-2 sm:grid-cols-1">
        <div
          class="md:w-full lg:w-full w-full sm:w-1/2 xl:w-fit flex flex-col sm:flex-row sm:px-6 py-6 sm:py-12 sm:space-x-10 sm:border-r-0 border-[#DDDDDD]"
        >
          <div class="sm:hidden xl:block mb-6 sm:mb-0">
            <a href="#">
              <img :src="require('~/assets/img/logo/nefa.svg')" class="w-24 -mt-2" alt="Nefa Logo" />
            </a>
          </div>
          <ul class="space-y-4">
            <NavLink name="Youtube" url="https://www.youtube.com/@meta" />
            <NavLink name="АФИША" url="https://xn--80aafkca5bdpa3bj2p.xn--p1ai/afisha/" />
            <NavLink name="Новости" url="https://xn--80aafkca5bdpa3bj2p.xn--p1ai/news/" />
          </ul>
        </div>
        <div
          class="md:w-full lg:w-full lg:border-r w-full sm:w-1/2 xl:w-fit sm:px-16 py-6 sm:py-12 border-t sm:border-t xl:border-r border-[#DDDDDD]"
        >
          <ul class="space-y-4">
            <NavLink name="Products" url="https://xn--80aafkca5bdpa3bj2p.xn--p1ai/metaverses/" />
          </ul>
        </div>

        <div
          class="md:w-full md:border-t lg:w-full sm:px-10 py-6 sm:py-12 w-full sm:w-1/2 xl:w-[22rem] space-y-4 sm:border-t border-[#DDDDDD]"
        >
          <h5 class="text-sm font-medium text-[#666666] focus:outline-none focus:shadow-outline">META</h5>
          <p class="text-sm text-[#666666] focus:outline-none focus:shadow-outline">
            Организация признана экстремистской и запрещена в РФ
          </p>
        </div>
      </div>
    </div>
    <div class="py-8 sm:py-4 text-center text-sm text-[#666666] hover:text-gray-900">
      &copy; Copyright 2023. All rights reserved
    </div>
  </footer>
</template>
<script>
export default {
  name: 'BaseFooter',
}
</script>
