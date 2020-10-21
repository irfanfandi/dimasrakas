<template>
  <div class="fixed inset-y-0 left-0 z-10 w-64 h-screen px-2 bg-light">
    <div class="h-screen pt-20 overflow-y-auto">
      <ul class="flex flex-col w-full">
        <li class="my-px">
          <nuxt-link
            to="/components/introduction"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Introduction</span>
          </nuxt-link>
          <nuxt-link
            to="/components"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Instalation</span>
          </nuxt-link>
          <nuxt-link
            to="/components"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Components</span>
          </nuxt-link>
        </li>
        <li class="my-px">
          <span
            class="flex p-2 px-4 mt-4 text-sm font-bold uppercase transition duration-200 cursor-pointer font-primary hover:bg-primary-alpha hover:text-primary rounded-10"
            @click="
              showUtilities ? (showUtilities = false) : (showUtilities = true)
            "
            >Utilities & Class</span
          >
        </li>
        <li v-show="showUtilities" class="my-px">
          <nuxt-link
            to="/components/atomics/color"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Color</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/shadow"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Shadow</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/rounded"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Rounded</span>
          </nuxt-link>
        </li>

        <!-- Atomic Components -->
        <li class="my-px">
          <span
            class="flex p-2 px-4 text-sm font-bold uppercase transition duration-200 cursor-pointer font-primary hover:bg-primary-alpha hover:text-primary rounded-10"
            @click="showAtomics ? (showAtomics = false) : (showAtomics = true)"
            >Atomic Components</span
          >
        </li>
        <li v-show="showAtomics" class="my-px">
          <nuxt-link
            to="/components/atomics/form"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Form</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/typography"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Typography</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/button"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Button</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/listview"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>List View</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Table</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Tab View</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Navigation</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Alert</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Badge</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Avatar</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Chips</span>
          </nuxt-link>
          <nuxt-link
            to="/components/atomics/table"
            class="flex flex-row items-center h-10 px-4 text-gray-600 transition duration-500 ease-in-out rounded-lg hover:text-primary hover:bg-primary-alpha"
          >
            <span>Tooltip</span>
          </nuxt-link>
        </li>

        <!-- Molecul Components -->
        <li class="my-px">
          <span class="flex px-4 mt-4 text-sm font-bold uppercase font-primary"
            >Molecul Components</span
          >
        </li>

        <!-- Organism Components -->
        <li class="my-px">
          <span class="flex px-4 mt-4 text-sm font-bold uppercase font-primary"
            >Organism Components</span
          >
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showUtilities: true,
      showAtomics: false,
    }
  },
}
</script>

<style></style>
