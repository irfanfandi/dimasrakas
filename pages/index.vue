<template>
  <section class="flex flex-col mt-16 space-y-6">
    <!-- Hero -->
    <div class="px-16">
      <div class="flex flex-wrap items-center">
        <div class="flex flex-wrap items-center w-1/2">
          <div class="flex flex-col space-y-10">
            <h1 class="font-extrabold leading-none font-primary text-display-3">
              Hello 👋
              <br />
              My Friends <br />Call me
              <span class="text-primary">Dimas</span>
            </h1>
            <p class="text-title-3 text-gray">
              We transform your business problems into beautiful creative
              solutions. Let us help you tell your story.
            </p>
          </div>
        </div>
        <div class="w-full md:w-1/2">
          <div class="flex items-center">
            <div class="w-4/12 px-3 space-y-6">
              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="block h-40 my-3 mb-2 overflow-hidden transition-all duration-500 transform scale-100 bg-white rounded-lg shadow-2xl hover:scale-95"
                >
                  <img
                    class="object-cover h-40"
                    src="/images/IMG_6985.jpg"
                    alt=""
                  />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="block h-40 my-3 mb-2 overflow-hidden transition-all duration-500 transform scale-100 bg-white rounded-lg shadow-2xl hover:scale-95"
                >
                  <img
                    class="object-cover h-40"
                    src="/images/IMG_7011.jpg"
                    alt=""
                  />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="block h-40 my-3 mb-2 overflow-hidden transition-all duration-500 transform scale-100 bg-white rounded-lg shadow-2xl hover:scale-95"
                >
                  <img
                    class="object-cover object-center w-full h-40"
                    src="/images/IMG_7003.jpg"
                    alt=""
                  />
                </div>
              </div>
            </div>
            <div class="w-8/12 px-3 space-y-6">
              <div v-scroll-reveal="{ delay: 800 }">
                <div
                  class="block my-3 mb-2 overflow-hidden transition-all duration-500 transform scale-100 bg-white rounded-lg shadow-2xl hover:scale-95"
                >
                  <img src="/images/IMG_6967.jpg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 900 }">
                <div
                  class="block my-3 mb-2 overflow-hidden transition-all duration-500 transform scale-100 rounded shadow-2xl hover:scale-95"
                >
                  <img src="/images/IMG_6996.jpg" alt="" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="p-16" style="background-color: #f9f9f9">
      <div class="flex flex-col space-y-8">
        <h1 class="font-bold leading-tight font-primary text-display-5">
          Digital products <br />for creative people
        </h1>

        <div class="flex flex-wrap -mx-4">
          <div class="w-1/3 p-4">
            <div class="w-full h-64 rounded-10 bg-gray"></div>
          </div>
          <div class="w-1/3 p-4">
            <div class="w-full h-64 rounded-10 bg-gray"></div>
          </div>
          <div class="w-1/3 p-4">
            <div class="w-full h-64 rounded-10 bg-gray"></div>
          </div>
        </div>
      </div>
    </div>

    <!-- The Weapon -->
    <div class="px-16 mt-12">
      <div
        class="flex flex-col items-center p-10 md:flex-row rounded-20 bg-primary"
      >
        <div
          class="flex flex-col items-center mb-16 text-center lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 md:items-start md:text-left md:mb-0"
        >
          <h1
            v-scroll-reveal="{ delay: 100 }"
            class="mb-4 font-bold leading-tight text-white font-primary text-display-5"
          >
            My Stack Weapon for Fight.
          </h1>
          <p
            v-scroll-reveal="{ delay: 200 }"
            class="leading-relaxed text-white text-subtitle-1"
          >
            With over 60+ YouTube videos, I have created a free educational
            community to help you learn UI/UX Design and more.
          </p>

          <div class="flex flex-wrap w-full -mx-4">
            <div class="w-1/2 p-4">
              <div class="w-16 h-16 rounded-10 bg-red"></div>
            </div>
            <div class="w-1/2 p-4">
              <div class="w-16 h-16 rounded-10 bg-red"></div>
            </div>
            <div class="w-1/2 p-4">
              <div class="w-16 h-16 rounded-10 bg-red"></div>
            </div>
            <div class="w-1/2 p-4">
              <div class="w-16 h-16 rounded-10 bg-red"></div>
            </div>
          </div>
        </div>
        <div class="w-full md:w-1/2">
          <div class="flex items-center justify-end mb-5">
            <div class="w-2/12 px-3 space-y-6">
              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/figma.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/whimsical.png" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/adobe-xd.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/adobe-photoshop.svg" alt="" />
                </div>
              </div>
            </div>
            <div class="w-2/12 px-3 space-y-6">
              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/vue-js.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/nuxt-js.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/react-js.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/next-js.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/tailwind-css.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/bootstrap.svg" alt="" />
                </div>
              </div>
            </div>
            <div class="w-2/12 px-3 space-y-6">
              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/laravel.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/codeigniter.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/express-js.svg" alt="" />
                </div>
              </div>
            </div>
            <div class="w-2/12 px-3 space-y-6">
              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/mysql.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/maria-db.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/sybase.jpg" alt="" />
                </div>
              </div>
            </div>
            <div class="w-2/12 px-3 space-y-6">
              <div v-scroll-reveal="{ delay: 500 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/digital-ocean.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 600 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/aws.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/netlify.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/open-litespeed.svg" alt="" />
                </div>
              </div>

              <div v-scroll-reveal="{ delay: 700 }">
                <div
                  class="flex items-center justify-center w-16 h-16 p-3 duration-500 transform scale-100 bg-white rounded-full shadow-2xl hover:scale-95"
                >
                  <img src="/weapon/nginx.svg" alt="" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Sources -->
    <div class="flex flex-wrap px-2">
      <div class="w-1/2 p-2">
        <div class="flex flex-col items-center justify-center p-4 bg-light">
          <div class="flex flex-col items-center justify-center my-8">
            <p class="text-gray text-title-4">Project</p>
            <h1 class="font-extrabold leading-none text-heading-1 font-primary">
              My Proffesional Project
            </h1>
            <p class="mt-4 text-center">
              Pay for your new Mac over 12 months, <br />
              interest‑free with Apple Card.
            </p>
            <nuxt-link to="/hr" class="mt-2 text-primary"
              >Selengkapnya ></nuxt-link
            >
          </div>
          <img class="h-72" src="~/assets/illustrations/woman.svg" alt="" />
        </div>
      </div>
      <div class="w-1/2 p-2">
        <div class="flex flex-col items-center justify-center p-4 bg-light">
          <div class="flex flex-col items-center justify-center my-8">
            <p class="text-gray text-title-4">Project</p>
            <h1 class="font-extrabold leading-none text-heading-1 font-primary">
              My Idealism Project
            </h1>
            <p class="mt-4 text-center">
              Pay for your new Mac over 12 months, <br />
              interest‑free with Apple Card.
            </p>
            <nuxt-link to="/hr" class="mt-2 text-primary"
              >Selengkapnya ></nuxt-link
            >
          </div>
          <img class="h-72" src="~/assets/illustrations/man.svg" alt="" />
        </div>
      </div>
      <div class="w-1/2 p-2">
        <div class="flex flex-col items-center justify-center p-4 bg-light">
          <div class="flex flex-col items-center justify-center my-8">
            <p class="text-gray text-title-4">Exercise</p>
            <h1 class="font-extrabold leading-none text-heading-1 font-primary">
              Redesign.
            </h1>
            <p class="mt-4 text-center">
              Pay for your new Mac over 12 months, <br />
              interest‑free with Apple Card.
            </p>
            <nuxt-link to="/hr" class="mt-2 text-primary"
              >Selengkapnya ></nuxt-link
            >
          </div>
          <img class="h-72" src="~/assets/illustrations/woman.svg" alt="" />
        </div>
      </div>
      <div class="w-1/2 p-2">
        <div class="flex flex-col items-center justify-center p-4 bg-light">
          <div class="flex flex-col items-center justify-center my-8">
            <p class="text-gray text-title-4">Exercise</p>
            <h1 class="font-extrabold leading-none text-heading-1 font-primary">
              Clone.
            </h1>
            <p class="mt-4 text-center">
              Pay for your new Mac over 12 months, <br />
              interest‑free with Apple Card.
            </p>
            <nuxt-link to="/hr" class="mt-2 text-primary"
              >Selengkapnya ></nuxt-link
            >
          </div>
          <img class="h-72" src="~/assets/illustrations/man.svg" alt="" />
        </div>
      </div>
    </div>

    <footer class="text-white border-t border-light">
      <div>
        <div
          class="container flex flex-col flex-wrap px-5 py-4 mx-auto sm:flex-row"
        >
          <p class="text-sm text-center text-gray-500 sm:text-left">
            © 2020 Qloud ID —
            <a
              href="#"
              rel="noopener noreferrer"
              class="ml-1 text-gray-600"
              target="_blank"
              >@ Surabaya</a
            >
          </p>
          <span
            class="inline-flex justify-center mt-2 sm:ml-auto sm:mt-0 sm:justify-start"
          >
            <a class="text-gray-500">
              <svg
                fill="currentColor"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                class="w-5 h-5"
                viewBox="0 0 24 24"
              >
                <path
                  d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z"
                ></path>
              </svg>
            </a>
            <a class="ml-3 text-gray-500">
              <svg
                fill="currentColor"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                class="w-5 h-5"
                viewBox="0 0 24 24"
              >
                <path
                  d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0023 3z"
                ></path>
              </svg>
            </a>
            <a class="ml-3 text-gray-500">
              <svg
                fill="none"
                stroke="currentColor"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                class="w-5 h-5"
                viewBox="0 0 24 24"
              >
                <rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect>
                <path
                  d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37zm1.5-4.87h.01"
                ></path>
              </svg>
            </a>
            <a class="ml-3 text-gray-500">
              <svg
                fill="currentColor"
                stroke="currentColor"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="0"
                class="w-5 h-5"
                viewBox="0 0 24 24"
              >
                <path
                  stroke="none"
                  d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6zM2 9h4v12H2z"
                ></path>
                <circle cx="4" cy="4" r="2" stroke="none"></circle>
              </svg>
            </a>
          </span>
        </div>
      </div>
    </footer>
  </section>
</template>

<script>
export default {}
</script>

<style></style>
