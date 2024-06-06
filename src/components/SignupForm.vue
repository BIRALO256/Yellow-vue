<template>
    <form  class="max-w-md mx-auto bg-white p-6 rounded-lg shadow-lg">
        <div class="mb-4">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="email">Email:</label>
        <input 
            type="email" 
            id="email" 
            required 
            v-model="email" 
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" 
        >
    </div>
    <div class="mb-4">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="password">Password:</label>
        <input 
            type="password" 
            id="password" 
            required 
            v-model="password" 
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" 
        >
    </div>

    <div class="mb-4">
      <label class="block text-gray-700 text-sm font-bold mb-2" for="role">Role:</label>
      <select
        id="role"
        required
        v-model="role"
        class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
      >
        <option value="" disabled>Select your role</option>
        <option value="Web Developer">Web Developer</option>
        <option value="Web Designer">Web Designer</option>
      </select>
    </div>

    <div class="mb-4 flex items-center">
      <input
        type="checkbox"
        id="terms"
        required
        v-model="acceptTerms"
        class="form-checkbox h-5 w-5 text-gray-600"
      >
      <label for="terms" class="ml-2 block text-gray-700 text-sm">Accept terms and conditions</label>
    </div>

    </form>
    <p>Email :{{email}}</p>
    <p>Passweord : {{ password }}</p>
    <p>Role : {{ role }}</p>

</template>

<script>
export default {
    data(){
        return{
            email : '',
            password : '',
            role : '',
        }
        
    }
}
</script>

<style>

</style>