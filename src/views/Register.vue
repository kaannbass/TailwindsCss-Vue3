<template>
  <div>
    <img class="mx-auto h-12 w-auto" src="https://tailwindui.com/img/logos/workflow-mark.svg?color=indigo&shade=600"
         alt="Workflow"/>
    <h2 class="mt-6 text-center text-3xl tracking-tight font-bold text-gray-900">Register For Free</h2>
    <p class="mt-2 text-center text-sm text-gray-600">
      Or
      {{ ' ' }}
      <router-link :to="{name:'Login'}" class="font-medium text-indigo-600 hover:text-indigo-500"> Login to your
        account
      </router-link>
    </p>
  </div>
  <form class="mt-5 space-y-6" action="#" method="POST">
    <div class="rounded-lg shadow-sm -space-y-px">
      <div class="mb-1">
        <label for="FullName" class="">Full Name</label>
        <input id="FullName" name="email" type="text" autocomplete="name" required=""
               class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-t-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm"
        />
      </div>
      <div class="mb-1">
        <label for="email-address" class="">Email address</label>
        <input id="email-address" name="email" type="email" autocomplete="email" required=""
               class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-t-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm"
        />
      </div>
      <div class="mb-1">
        <label for="password" class="">Password</label>
        <input id="password" name="password" type="password" autocomplete="current-password" required=""
               class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-b-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm"
        />
      </div>
      <div class="mb-1">
        <label for="password" class="">Password Confirmation</label>
        <input id="passwordR" name="password" type="password" autocomplete="current-password" required=""
               class="appearance-none rounded-none relative block w-full px-3 py-2 border border-gray-300 placeholder-gray-500 text-gray-900 rounded-b-md focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 focus:z-10 sm:text-sm"
        />
      </div>
    </div>
    <div>
      <button type="submit"
              class="group relative w-full flex justify-center py-2 px-4 border border-transparent text-sm font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500">
            <span class="absolute left-0 inset-y-0 flex items-center pl-3">
              <LockClosedIcon class="h-5 w-5 text-indigo-500 group-hover:text-indigo-400" aria-hidden="true"/>
            </span>
        Sign up
      </button>
    </div>
  </form>
</template>

<script>
import { LockClosedIcon } from '@heroicons/vue/solid'
export default {
  name: 'Register',
  components:{
    LockClosedIcon
  }
}
</script>

<style scoped>

</style>