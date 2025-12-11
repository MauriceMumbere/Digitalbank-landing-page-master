<template>
  <footer class="bg-blue-950 text-white">
    <div class="px-6 md:px-32 py-16 flex flex-col md:flex-row md:justify-between space-y-12 md:space-y-0">

      <div class="flex flex-col items-center md:items-start md:flex-row space-y-12 md:space-y-0 md:space-x-24">

        <div class="flex flex-col items-center md:items-start space-y-6">
          <img src="/images/logo-light.svg" alt="Logo light" class="w-40">
          <ul class="flex space-x-4">
            <li><img src="/images/icon-facebook.svg" alt="Facebook"></li>
            <li><img src="/images/icon-youtube.svg" alt="YouTube"></li>
            <li><img src="/images/icon-twitter.svg" alt="Twitter"></li>
            <li><img src="/images/icon-pinterest.svg" alt="Pinterest"></li>
            <li><img src="/images/icon-instagram.svg" alt="Instagram"></li>
          </ul>
        </div>

        <div class="flex flex-col md:flex-row items-center md:items-start space-y-6 md:space-y-0 md:space-x-24 text-center md:text-left">

          <ul class="space-y-3 text-lg">
            <li><a href="#" class="hover:text-emerald-500 transition">About Us</a></li>
            <li><a href="#" class="hover:text-emerald-500 transition">Contact</a></li>
            <li><a href="#" class="hover:text-emerald-500 transition">Blog</a></li>
          </ul>

          <ul class="space-y-3 text-lg">
            <li><a href="#" class="hover:text-emerald-500 transition">Careers</a></li>
            <li><a href="#" class="hover:text-emerald-500 transition">Support</a></li>
            <li><a href="#" class="hover:text-emerald-500 transition">Privacy Policy</a></li>
          </ul>

        </div>
      </div>

      <div class="flex flex-col items-center md:items-end space-y-4 text-center md:text-right">
        <a href="#"
           class="relative overflow-hidden
          bg-linear-to-bl from-green-500 to-cyan-500
          py-3 px-7 rounded-4xl inline-block
          before:content-[''] before:absolute before:inset-0
          before:bg-transparent
          before:transition-all before:duration-200
          hover:before:bg-gray-50/40">
          Request Invite
        </a>

        <p class="text-sm text-gray-600">© Digitalbank. All Rights Reserved</p>
      </div>

    </div>
  </footer>
</template>
