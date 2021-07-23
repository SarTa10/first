<template>
    <div class="flex flex-col justify-center items-center">
        <h1 class="text-6xl tracking-widest"> Sing in</h1>
        <div class="flex my-4"> 
            <p class="text-base tracking-widest">If you don't have account please <nuxt-link
             to='/' class="text-blue-800 text-base tracking-wider" > sign up</nuxt-link></p>
        </div>

        <form action="" class="flex flex-col w-4/5 sm:w-96 justify-center items-center">
        <div class=" relative w-full">
            <input id="email" name="email" type="text" class="peer text-sm h-10 w-full border-2 rounded-lg input border-gray-300 text-gray-900 placeholder-transparent focus:outline-none focus:border-rose-600 p-3" placeholder="john@doe.com" />
            <label for="email" class="absolute left-1 top-4 text-gray-600 text-sm transition-all peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 peer-placeholder-shown:top-2.5 peer-focus:-top-1 peer-focus:text-gray-600 peer-focus:text-xs">Email address</label>
        </div>

        <div class=" relative mt-3 mb-3 w-full">
            <input id="email" name="email" type="password" class="peer text-sm h-10 w-full border-2 rounded-lg input border-gray-300 text-gray-900 placeholder-transparent focus:outline-none focus:border-rose-600 p-3" placeholder="john@doe.com" />
            <label for="email" class="absolute left-1 top-4 text-gray-600 text-sm transition-all peer-placeholder-shown:text-base peer-placeholder-shown:text-gray-400 peer-placeholder-shown:top-2.5 peer-focus:-top-1 peer-focus:text-gray-600 peer-focus:text-xs">password</label>
        </div>
            <div class="flex justify-between w-full">
                <div >
                    <input type="checkbox" >
                    <label class="text-gray-600"> Remember me</label>
                </div>

                <nuxt-link class="text-blue-800" to="/"> forgot password</nuxt-link>
            </div>

            <button class="w-full bg-black text-white mt-4 mb-4 rounded-md sign-in">sign in</button>   
        </form>

        <p class="mb-4">or sign in with</p>
        <button class="w-4/5 sm:w-96 sign-in border-2 border-gray-600 rounded-md mb-2">google</button>
        <button class="w-4/5 sm:w-96 sign-in border-2 border-gray-600 rounded-md">facebook</button>
    </div>
</template>

<script>
export default {}
</script>

<style >
    *{
        font-family:GT America Mono
    }

    button{
        font-family:GT America
    }

    .input{
        height:56px;
        position:relative
    }

    .sign-in{
        height:48px;
    }

input:focus-within ~ label,
input:not(:placeholder-shown) ~ label {
  @apply transform scale-75 -translate-y-4;
}

input:focus-within ~ label {
  @apply text-gray-500;
}

</style>