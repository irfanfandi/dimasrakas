<template>
  <div class="z-50 flex flex-col w-full">
    <div class="z-50 bg-white border-b-2 border-light shadow-20">
      <div class="px-4 mx-auto max-w-7xl sm:px-6">
        <div
          class="flex items-center justify-between py-2 md:justify-start md:space-x-10"
        >
          <div class="lg:w-0 lg:flex-1">
            <a href="#" class="flex">
              <img
                class="w-auto h-6 sm:h-6"
                src="https://dimasrakas.netlify.app/_nuxt/img/dimasrakas-logo.ae7c7f3.svg"
                alt="Workflow"
              />
            </a>
          </div>
          <div ref="collabsibles" class="-my-2 -mr-2 md:hidden">
            <button
              type="button"
              class="inline-flex items-center justify-center p-2 transition duration-150 ease-in-out rounded-md hover: hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:"
              @click="showMobileMenu = true"
            >
              <!-- Heroicon name: menu -->
              <svg
                class="w-6 h-6"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M4 6h16M4 12h16M4 18h16"
                />
              </svg>
            </button>
          </div>
          <div class="hidden space-x-4 md:flex">
            <nuxt-link
              to="/"
              class="px-4 py-2 transition duration-150 ease-in-out rounded-10 hover:bg-primary-alpha text-tittle-2 hover:text-primary focus:outline-none focus:text-primary"
            >
              Home
            </nuxt-link>

            <!-- Components -->
            <div ref="collabsibles" class="relative">
              <button
                type="button"
                class="inline-flex items-center px-4 py-2 transition duration-150 ease-in-out rounded-10 hover:bg-primary-alpha text-tittle-2 group hover:text-primary focus:outline-none focus:text-primary"
                @click="
                  showComponents
                    ? (showComponents = false)
                    : showComponentsMenu()
                "
              >
                <span>MyProject </span>
                <svg
                  class="w-5 h-5 transition duration-150 ease-in-out group-hover: group-focus:"
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                >
                  <path
                    fill-rule="evenodd"
                    d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                    clip-rule="evenodd"
                  />
                </svg>
              </button>

              <ZoomFadeTransition>
                <div
                  v-show="showComponents"
                  class="absolute z-50 w-screen max-w-xs px-2 mt-3 -ml-4 transform sm:px-0 lg:ml-0 lg:left-1/2 lg:-translate-x-1/2"
                >
                  <div class="rounded-lg shadow-lg">
                    <div class="overflow-hidden rounded-lg shadow-xs">
                      <div
                        class="relative z-20 grid gap-6 px-5 py-4 bg-white sm:gap-8 sm:p-8"
                      >
                        <div
                          class="flex items-start p-2 -m-3 space-x-4 transition duration-150 ease-in-out rounded-lg hover:bg-primary-alpha"
                          @click="changePage('introduction')"
                        >
                          <svg
                            class="flex-shrink-0 w-6 h-6 text-primary"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              stroke-width="2"
                              d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"
                            />
                          </svg>
                          <div class="space-y-1">
                            <p class="text-tittle-2">Proffesional Project</p>
                          </div>
                        </div>
                        <div
                          class="flex items-start p-2 -m-3 space-x-4 transition duration-150 ease-in-out rounded-lg hover:bg-primary-alpha"
                          @click="changePage('utilities')"
                        >
                          <!-- Heroicon name: view-grid -->
                          <svg
                            class="flex-shrink-0 w-6 h-6 text-primary"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              stroke-width="2"
                              d="M4 6a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2H6a2 2 0 01-2-2V6zM14 6a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V6zM4 16a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2H6a2 2 0 01-2-2v-2zM14 16a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"
                            />
                          </svg>
                          <div class="space-y-1">
                            <p class="text-tittle-2">Idealism Project</p>
                          </div>
                        </div>
                        <hr />
                        <div
                          class="flex items-start p-2 -m-3 space-x-4 transition duration-150 ease-in-out rounded-lg hover:bg-primary-alpha"
                          @click="changePage('atomics')"
                        >
                          <!-- Heroicon name: cursor-click -->
                          <svg
                            class="flex-shrink-0 w-6 h-6 text-primary"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              stroke-width="2"
                              d="M15 15l-2 5L9 9l11 4-5 2zm0 0l5 5M7.188 2.239l.777 2.897M5.136 7.965l-2.898-.777M13.95 4.05l-2.122 2.122m-5.657 5.656l-2.12 2.122"
                            />
                          </svg>
                          <div class="space-y-1">
                            <p class="text-tittle-2">Qloud Universe</p>
                          </div>
                        </div>
                        <div
                          class="flex items-start p-2 -m-3 space-x-4 transition duration-150 ease-in-out rounded-lg hover:bg-primary-alpha"
                          @click="changePage('molecul')"
                        >
                          <!-- Heroicon name: shield-check -->
                          <svg
                            class="flex-shrink-0 w-6 h-6 text-primary"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              stroke-width="2"
                              d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"
                            />
                          </svg>
                          <div class="space-y-1">
                            <p class="text-tittle-2">Qloud Design System</p>
                          </div>
                        </div>
                        <div
                          class="flex items-start p-2 -m-3 space-x-4 transition duration-150 ease-in-out rounded-lg hover:bg-primary-alpha"
                          @click="changePage('molecul')"
                        >
                          <!-- Heroicon name: shield-check -->
                          <svg
                            class="flex-shrink-0 w-6 h-6 text-primary"
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                          >
                            <path
                              stroke-linecap="round"
                              stroke-linejoin="round"
                              stroke-width="2"
                              d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"
                            />
                          </svg>
                          <div class="space-y-1">
                            <p class="text-tittle-2">Tailwindow</p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </ZoomFadeTransition>
            </div>

            <!-- Icons -->
            <nuxt-link
              to="/icons"
              class="px-4 py-2 transition duration-150 ease-in-out hover:bg-primary-alpha rounded-10 text-tittle-2 hover:text-primary focus:outline-none focus:text-primary"
            >
              Weapon
            </nuxt-link>

            <nuxt-link
              to="/illustrations"
              class="px-4 py-2 transition duration-150 ease-in-out hover:bg-primary-alpha rounded-10 text-tittle-2 hover:text-primary focus:outline-none focus:text-primary"
            >
              Redesign
            </nuxt-link>

            <nuxt-link
              to="/collections"
              class="px-4 py-2 transition duration-150 ease-in-out hover:bg-primary-alpha rounded-10 text-tittle-2 hover:text-primary focus:outline-none focus:text-primary"
            >
              Clone
            </nuxt-link>
          </div>

          <div
            class="items-center justify-end hidden space-x-8 md:flex md:flex-1 lg:w-0"
          >
            <a
              href="#"
              class="whitespace-no-wrap text-tittle-2 hover:text-primary focus:outline-none focus:text-primary"
            >
              Github
            </a>
          </div>
        </div>
      </div>

      <ZoomFadeTransition>
        <div
          v-show="showMobileMenu"
          class="absolute inset-x-0 top-0 p-2 transition origin-top-right transform md:hidden"
        >
          <div class="rounded-lg shadow-lg">
            <div
              class="bg-white divide-y-2 rounded-lg shadow-xs divide-gray-50"
            >
              <div class="px-5 pt-5 pb-6 space-y-6">
                <div class="flex items-center justify-between">
                  <div>
                    <img
                      class="w-auto h-8"
                      src="https://tailwindui.com/img/logos/workflow-mark-on-white.svg"
                      alt="Workflow"
                    />
                  </div>
                  <div class="-mr-2">
                    <button
                      type="button"
                      class="inline-flex items-center justify-center p-2 transition duration-150 ease-in-out rounded-md hover: hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:"
                      @click="showMobileMenu = false"
                    >
                      <!-- Heroicon name: x -->
                      <svg
                        class="w-6 h-6"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          stroke-width="2"
                          d="M6 18L18 6M6 6l12 12"
                        />
                      </svg>
                    </button>
                  </div>
                </div>
                <div>
                  <nav class="grid gap-y-8">
                    <a
                      href="#"
                      class="flex items-center p-3 -m-3 space-x-3 transition duration-150 ease-in-out rounded-md hover:bg-primary-alpha"
                    >
                      <!-- Heroicon name: chart-bar -->
                      <svg
                        class="flex-shrink-0 w-6 h-6 text-primary"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          stroke-width="2"
                          d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"
                        />
                      </svg>
                      <div class="text-tittle-2">Qloud POS</div>
                    </a>
                    <a
                      href="#"
                      class="flex items-center p-3 -m-3 space-x-3 transition duration-150 ease-in-out rounded-md hover:bg-primary-alpha"
                    >
                      <!-- Heroicon name: cursor-click -->
                      <svg
                        class="flex-shrink-0 w-6 h-6 text-primary"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          stroke-width="2"
                          d="M15 15l-2 5L9 9l11 4-5 2zm0 0l5 5M7.188 2.239l.777 2.897M5.136 7.965l-2.898-.777M13.95 4.05l-2.122 2.122m-5.657 5.656l-2.12 2.122"
                        />
                      </svg>
                      <div class="text-tittle-2">Qloud HR</div>
                    </a>
                    <a
                      href="#"
                      class="flex items-center p-3 -m-3 space-x-3 transition duration-150 ease-in-out rounded-md hover:bg-primary-alpha"
                    >
                      <!-- Heroicon name: shield-check -->
                      <svg
                        class="flex-shrink-0 w-6 h-6 text-primary"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          stroke-width="2"
                          d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"
                        />
                      </svg>
                      <div class="text-tittle-2">Qloud Sales</div>
                    </a>
                    <a
                      href="#"
                      class="flex items-center p-3 -m-3 space-x-3 transition duration-150 ease-in-out rounded-md hover:bg-primary-alpha"
                    >
                      <!-- Heroicon name: view-grid -->
                      <svg
                        class="flex-shrink-0 w-6 h-6 text-primary"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          stroke-width="2"
                          d="M4 6a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2H6a2 2 0 01-2-2V6zM14 6a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V6zM4 16a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2H6a2 2 0 01-2-2v-2zM14 16a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"
                        />
                      </svg>
                      <div class="text-tittle-2">QloudX</div>
                    </a>
                    <a
                      href="#"
                      class="flex items-center p-3 -m-3 space-x-3 transition duration-150 ease-in-out rounded-md hover:bg-primary-alpha"
                    >
                      <!-- Heroicon name: refresh -->
                      <svg
                        class="flex-shrink-0 w-6 h-6 text-primary"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                      >
                        <path
                          stroke-linecap="round"
                          stroke-linejoin="round"
                          stroke-width="2"
                          d="M4 4v5h.582m15.356 2A8.001 8.001 0 004.582 9m0 0H9m11 11v-5h-.581m0 0a8.003 8.003 0 01-15.357-2m15.357 2H15"
                        />
                      </svg>
                      <div class="text-tittle-2">Automations</div>
                    </a>
                  </nav>
                </div>
              </div>
              <div class="px-5 py-6 space-y-6">
                <div class="grid grid-cols-2 gap-y-4 gap-x-8">
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Harga
                  </a>
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Bantuan
                  </a>
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Enterprise
                  </a>
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Blog
                  </a>
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Help Center
                  </a>
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Guides
                  </a>
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Security
                  </a>
                  <a
                    href="#"
                    class="transition duration-150 ease-in-out text-tittle-2 text-primary hover:text-gray-700"
                  >
                    Events
                  </a>
                </div>
                <div class="space-y-6">
                  <span class="flex w-full rounded-md shadow-sm">
                    <a
                      href="#"
                      class="flex items-center justify-center w-full px-4 py-2 text-white transition duration-150 ease-in-out border border-transparent rounded-md text-tittle-2 bg-primary hover:bg-primary-alpha focus:outline-none focus:border-indigo-700 focus:shadow-outline-indigo active:bg-indigo-700"
                    >
                      Sign up
                    </a>
                  </span>
                  <p class="text-center text-tittle-2">
                    Existing customer?
                    <a
                      href="#"
                      class="transition duration-150 ease-in-out text-primary hover:text-indigo-500"
                    >
                      Sign in
                    </a>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </ZoomFadeTransition>
    </div>
  </div>
</template>

<script>
import ZoomFadeTransition from '~/components/Transitions/ZoomFade'
export default {
  components: {
    ZoomFadeTransition,
  },
  data() {
    return {
      showComponents: false,
      showMore: false,
      showMobileMenu: false,
    }
  },
  mounted() {
    document.addEventListener('click', this.onClickOutside)
  },
  methods: {
    hideAll() {
      this.showComponents = false
      this.showMore = false
      this.showMobileMenu = false
    },
    showComponentsMenu() {
      this.showComponents = true
      this.showMore = false
    },
    showMoreMenu() {
      this.showMore = true
      this.showComponents = false
    },
    onClickOutside(event) {
      const { collabsibles } = this.$refs
      if (!collabsibles || collabsibles.contains(event.target)) return
      this.hideAll()
    },
    changePage(name) {
      this.$router.push('/components/' + name)
      this.showComponents = false
    },
  },
}
</script>

<style></style>
