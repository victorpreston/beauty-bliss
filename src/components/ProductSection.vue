<template>
    <section id="products" class="py-6 bg-gray-200">
        <!-- search container -->
        <div class="container mx-auto px-6">
            <!-- search & filter -->
            <div class="w-full mx-auto flex flex-col justify-center space-y-4 md:flex-row md:space-y-0 md:space-x-4 ">
                <div class="md:w-1/2 flex items-center justify-center">
                    <input type="search"
                        class="w-full px-4 py-2.5 border border-gray-300 outline-none focus:ring-1 focus:ring-cyan-700 rounded-l-lg"
                        placeholder="Search products....">
                    <button
                        class="flex items-center text-white gap-x-2 px-4 py-2.5 border border-cyan-700 bg-cyan-700 hover:opacity-90 rounded-r-lg cursor-pointer">
                        <span>
                            <svg class="w-6 h-6 text-white" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                                width="24" height="24" fill="none" viewBox="0 0 24 24">
                                <path stroke="currentColor" stroke-linecap="round" stroke-width="2"
                                    d="m21 21-3.5-3.5M17 10a7 7 0 1 1-14 0 7 7 0 0 1 14 0Z" />
                            </svg>
                        </span>
                        Search
                    </button>
                </div>
                <div>
                    <label for="category" class="sr-only">Category</label>
                    <select name="category" id="category"
                        class="w-full px-4 py-2.5 border border-gray-300 rounded-lg focus:ring-1 focus:ring-cyan-700 focus:outline-none">
                        <option class="appearance-none hover:bg-cyan-700" selected>All filters</option>
                        <option value="MU">Makeup</option>
                        <option value="SC">Skincare</option>
                        <option value="BB">Bath & Body</option>
                        <option value="FR">Fragrance</option>
                    </select>
                </div>
            </div>
        </div>
        <!-- end search container -->

        <!-- quick shop section -->
        <QuickShop />

        <!-- products container -->
        <div class="container mx-auto my-12 px-8 md:px-12 xl:px-36">

            <!-- trending products -->
            <div class="capitalize flex items-center justify-between">
                <h3 class="text-xl font-bold md:text-2xl">all products</h3>
                <a href="#"
                    class="hidden text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200 md:block">
                    Show all
                </a>
            </div>

            <!-- products -->
            <div class="mt-8 grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-4">
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/avon1.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class=" text-cyan-700 uppercase font-bold line-clamp-1 md:text-lg">avon care derma</h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Moisturise, brighten, perfect and protect your skin with Avon Care Derma Even-Tone+ Radiance
                            Body Lotion.
                        </p>

                        <div class="w-fit mt-2 bg-green-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">10+ pcs In stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K15,000</h4>
                                <span class="text text-gray-500 line-through">K20,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/avon2.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class=" text-cyan-700 uppercase font-bold line-clamp-1 md:text-lg">avon far away rebel</h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Dare to be real. With Far Away Rebel Body Lotion and its oriental and floral scent, you can
                            be whatever you want to be.
                        </p>

                        <div class="w-fit mt-2 bg-green-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">30+ pcs In stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K50,000</h4>
                                <span class="text text-gray-500 line-through">K80,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/avon3.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class=" text-cyan-700 uppercase font-bold line-clamp-1 md:text-lg">avon anew skin renewal
                        </h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Start feeling firmer, more supple skin in just 2 days* by adding Anew Ultimate Firm & Supple
                            Day Cream to your skincare regime.
                        </p>

                        <div class="w-fit mt-2 bg-red-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">out of stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K125,000</h4>
                                <span class="text text-gray-500 line-through">K160,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/gucci1.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class=" text-cyan-700 uppercase font-bold md:text-lg">Gucci Memoire</h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Gucci Memoire d'une Odeur Eau de Parfum is a herbal and woody fragrance
                            for men and women. Classed as a floral, musky
                            and powdery scent.
                        </p>

                        <div class="w-fit mt-2 bg-green-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">50+ pcs In stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K285,000</h4>
                                <span class="text text-gray-500 line-through">K300,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer  hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/avon4.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class=" text-cyan-700 uppercase font-bold md:text-lg">Avon Care Cocoa Butter</h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Nourish and smooth normal to extra dry skin with Avon Care Cocoa Nourishing Body Lotion and
                            its deeply hydrating cocoa butter blend.
                        </p>

                        <div class="w-fit mt-2 bg-green-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">3+ pcs In stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K85,000</h4>
                                <span class="text text-gray-500 line-through">K100,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer  hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/avon5.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class="text-cyan-700 uppercase font-bold md:text-lg line-clamp-1">Avon Care Essential
                            Moisture</h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Leaves skin looking & feeling intensely nourished & protected from dryness. With glycerin &
                            almond milk + vitamin E.
                        </p>

                        <div class="w-fit mt-2 bg-green-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">11+ pcs In stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K35,000</h4>
                                <span class="text text-gray-500 line-through">K48,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer  hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/avon6.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class="text-cyan-700 uppercase font-bold md:text-lg line-clamp-1">Avon Ultra Volume
                            Waterproof Mascara</h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Want instant bold volume that lasts all day? Get it with Ultra Volume Waterproof Mascara.
                        </p>

                        <div class="w-fit mt-2 bg-green-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">80+ pcs In stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K55,000</h4>
                                <span class="text text-gray-500 line-through">K72,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer  hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->
                <!-- product card -->
                <div class="relative bg-white mx-auto flex flex-col justify-center shadow-lg rounded-lg">
                    <!-- product image -->
                    <div class="border-b-2 border-gray-200 overflow-hidden">
                        <a href="#" class="">
                            <img src="@/assets/images/avon7.jpg" alt=""
                                class="w-full h-60 object-contain object-center rounded-t-lg hover:scale-110 duration-200">
                        </a>
                    </div>
                    <!-- product details -->
                    <div class="px-4 py-4">
                        <h3 class="text-cyan-700 uppercase font-bold md:text-lg line-clamp-1">Foot Works Lavender</h3>
                        <p class="text-sm text-gray-500 mt-2 line-clamp-2">
                            Moisturise, condition and soften your feet with this Foot Works Overnight Treatment.
                        </p>

                        <div class="w-fit mt-2 bg-green-200 px-2 py-1 rounded-lg">
                            <h4 class="text-xs text-gray-500">100+ pcs In stock</h4>
                        </div>

                        <div class="flex flex-col items-start mt-4 space-y-4">
                            <div class="w-full flex items-center justify-between">
                                <h4 class="text-2xl font-bold md:text-2xl ">K10,000</h4>
                                <span class="text text-gray-500 line-through">K26,000</span>
                            </div>
                            <button type="button"
                                class="group text-sm text-cyan-700 font-medium uppercase w-full flex items-center justify-center gap-x-2 px-4 py-2.5 border border-cyan-700 rounded-lg cursor-pointer  hover:bg-cyan-700 hover:text-white hover:border-cyan-700">
                                <span>
                                    <svg class="w-5 h-5 text-cyan-700 group-hover:text-white" aria-hidden="true"
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                            stroke-width="2"
                                            d="M5 4h1.5L9 16m0 0h8m-8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm8 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4Zm-8.5-3h9.25L19 7H7.312" />
                                    </svg>
                                </span>
                                Add to cart
                            </button>
                        </div>
                    </div>
                </div>
                <!-- end product card -->

            </div>

            <div class="w-full mx-auto mt-8 flex items-center justify-center md:hidden">
                <a href="#"
                    class="text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200">
                    Show all
                </a>
            </div>
            <!-- end products -->
        </div>
        <!-- end products container -->
    </section>
</template>

<script setup>
import QuickShop from '@/components/QuickShop.vue'
</script>
