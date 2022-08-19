<template>
  <div className="min-h-full flex items-center justify-center py-12 px-4 sm:px-6 lg:px-8">
    <div className="max-w-md w-full space-y-8">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import {LockClosedIcon} from '@heroicons/vue/solid'

export default {
  name: 'AuthLayout',
}
</script>

<style scoped>

</style>