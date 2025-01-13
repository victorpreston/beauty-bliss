<template>
    <!-- quick shop section -->
    <section>
        <!-- quick shop container -->
        <div class="container mx-auto my-12 px-8 md:px-12 xl:px-36">
            <!-- heading -->
            <div class="capitalize flex items-center justify-between mb-6">
                <h3 class="text-xl font-bold md:text-2xl">new arrivals</h3>
                <a href="#"
                    class="hidden text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200 md:block">
                    Show all
                </a>
            </div>

            <!-- item container -->
            <div class="bg-cyan-100 grid grid-cols-1 gap-6 md:grid-cols-3 md:grid-rows-2 p-8">
                <!-- item 1 -->
                <div class="grid grid-cols-1 md:grid-cols-2 gap-6 rounded-lg md:col-span-2 md:row-span-2">
                    <!-- sub item -->
                    <div class="group relative bg-white rounded-lg md:col-span-2">
                        <img src="../assets/images/quickshop1.jpg" alt=""
                            class="w-full h-60 object-contain rounded-xl shadow-lg">

                        <div
                            class="absolute top-2 left-2 px-4 py-1 text-white bg-cyan-700 rounded-lg opacity-0 group-hover:opacity-100 duration-200">
                            50% off
                        </div>

                        <div
                            class="absolute bottom-0 flex items-center justify-center bg-gray-200 rounded-b-lg w-full opacity-0 p-4 group-hover:opacity-100 duration-200">
                            <a href="#"
                                class="text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200">Shop
                                Now</a>
                        </div>
                    </div>
                    <!-- end sub item -->
                    <!-- sub item -->
                    <div class="group relative bg-white rounded-lg">
                        <img src="../assets/images/quickshop2.jpg" alt=""
                            class="w-full h-60 object-contain rounded-xl shadow-lg">

                        <div
                            class="absolute top-2 left-2 px-4 py-1 text-white bg-cyan-700 rounded-lg opacity-0 group-hover:opacity-100 duration-200">
                            25% off
                        </div>

                        <div
                            class="absolute bottom-0 flex items-center justify-center bg-gray-200 rounded-b-lg w-full opacity-0 p-4 group-hover:opacity-100 duration-200">
                            <a href="#"
                                class="text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200">Shop
                                Now</a>
                        </div>
                    </div>
                    <!-- end sub item -->
                    <!-- sub item -->
                    <div class="group relative bg-white rounded-lg">
                        <img src="../assets/images/quickshop3.jpg" alt=""
                            class="w-full h-60 object-contain rounded-xl shadow-lg">

                        <div
                            class="absolute top-2 left-2 px-4 py-1 text-white bg-cyan-700 rounded-lg opacity-0 group-hover:opacity-100 duration-200">
                            5% off
                        </div>

                        <div
                            class="absolute bottom-0 flex items-center justify-center bg-gray-200 rounded-b-lg w-full opacity-0 p-4 group-hover:opacity-100 duration-200">
                            <a href="#"
                                class="text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200">Shop
                                Now</a>
                        </div>
                    </div>
                    <!-- end sub item -->

                </div>
                <!-- end item 1 -->

                <!-- item 2 -->
                <div class="group relative bg-white rounded-lg md:row-span-2">
                    <img src="../assets/images/quickshop4.jpg" alt=""
                        class="w-full h-60 md:h-full object-contain rounded-xl shadow-lg">

                    <div
                        class="absolute top-2 left-2 px-4 py-1 text-white bg-cyan-700 rounded-lg opacity-0 group-hover:opacity-100 duration-200">
                        25% off
                    </div>

                    <div
                        class="absolute bottom-0 flex items-center justify-center bg-gray-200 rounded-b-lg w-full opacity-0 p-4 group-hover:opacity-100 duration-200">
                        <a href="#"
                            class="text-cyan-700 uppercase px-4 py-2 border border-cyan-700 rounded-lg hover:bg-cyan-700 hover:text-white hover:border-cyan-700 duration-200">Shop
                            Now</a>
                    </div>
                </div>
                <!-- end item 2 -->
            </div>
            <!-- end item container -->
        </div>
        <!-- end quick shop container -->
    </section>
</template>