<template>
  <div class="container mx-auto h-screen flex justify-center items-center">
    <div class="w-full lg:w-1/3 px-10 lg:px-0">
      <div class="flex justify-center items-center mx-auto mt-6 mb-8">
        <img
          src="../../static/error-illustration.svg"
          height="370"
          width="424"
          alt=""
          class="w-full"
        />
      </div>
      <h2 class="font-medium mb-3 text-3xl text-center">
        Oppsss. Something wrong
      </h2>
      <p class="text-center font-light">
        An error occured when processing your transaction <br />
        Please try again later
      </p>
      <div class="mb-4 mt-6">
        <div class="mb-3">
          <button
            @click="$router.push({ path: '/' })"
            class="block w-full bg-orange-button hover:bg-green-button text-white font-semibold px-6 py-4 text-lg rounded-full"
          >
            Fund Other Project
          </button>
        </div>
        <div class="mb-4">
          <button
            @click="$router.push({ path: '/dashboard' })"
            class="block w-full bg-transparent border border-gray-500 text-gray-500 hover:bg-green-button hover:border-green-button hover:text-white font-light px-6 py-4 text-lg rounded-full"
          >
            My Dashboard
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'success',
}
</script>
