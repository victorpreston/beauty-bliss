<template>
    <section class="bg-cyan-50">
        <!-- cta container -->
        <div class="container  mx-auto p-16 px-8 md:px-12 xl:px-36">
            <div class=" flex flex-col items-center justify-center space-y-6 ">
                <div class="text-center">
                    <h3 class="text-2xl text-cyan-700 font-bold md:text-3xl">Subscribe to our newsletter</h3>
                    <p class="text-sm text-gray-500 mt-2">Sign up for our newsletter and receive exclusive offers and
                        discounts.</p>
                </div>

                <div class="flex flex-col w-full mx-auto space-y-6 items-center">
                    <input type="email"
                        class="w-full px-4 py-2.5 border border-gray-300 outline-none focus:ring-1 focus:ring-cyan-700 rounded-lg placeholder:text-center md:w-1/2 "
                        placeholder="Enter your email" required>
                    <button type="submit"
                        class="block w-fit text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200 cursor-pointer">
                        Subscribe
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>