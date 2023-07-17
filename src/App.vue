<script setup>
import image from './assets/Hero.png'
import image2 from './assets/logo.png'
import image3 from './assets/Iphone-Mockup.png'
import image4 from './assets/Feature-Background.png'

const title = ["Budgeting made simple", "Works beautifully on your iOS device"]
const summry = ["Numm uses an envelope budgeting style where each expense has its own envelope.", "Getting out of debt and saving more money has never been this easy."]
const arryObj = [
    "Payees", "Categories", "Scheduled transactions", "Multiple budgets", "Goal tracking", "Sync between devices", "Reports", "Sync with your bank",
    { headline: ["Create payees for your most commonly used payment destinations.", "Group similar transaction destinations for easier operation.", "Get notified ahead of time of due transactions.", "You can seamlessly switch from a personal budget to a company one.", "Track your transactions and updates the goals you set for various categories.", "All your data will be synced seamlessly between iOS devices.", "Generate insighful reports for your spending habits but also for income trends. Also export to PDF.", "Grab all the transactions from your bank statement automatically."] }
]

</script>

<template>
    <section class="container mx-auto">
        <header class=" px-4 py-10" :style="`background: url(${image}) no-repeat; background-size: cover; height: 1000px;`">
            <div class="header-hero">
                <div class="logo-menu flex items-center gap-5">
                    <div class="logo basis-1/12">
                        <img :src="image2" alt="">
                    </div>
                    <div class="menu basis-11/12">
                        <ul class="flex gap-10 text-white font-bold">
                            <li>
                                <a href="#">Screesnshots</a>
                            </li>
                            <li>
                                <a href="#">Testimonials</a>
                            </li>
                            <li>
                                <a href="#">Pricing</a>
                            </li>
                            <li>
                                <a href="#">Features</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="grid grid-cols-12 gap-4 pt-8">
                <div class="col-start-2 col-span-6">
                    <div class="banner-text mx-auto px-4 py-10">
                        <h1 class="text-4xl font-bold text-white">{{ title[0] }}</h1>
                        <p class="text-white py-6 ">{{ summry[0] }}</p>
                        <div class="my-8">
                            <button
                                class="py-2 px-4 bg-blue-500 text-white font-semibold rounded-lg shadow-md hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-400 focus:ring-opacity-75">
                                Download for free
                            </button>
                            <button
                                class="bg-transparent text-white hover:bg-blue-700 font-bold py-2 px-4 border border-none rounded-lg">
                                Video introduction
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </header>
        <main>
            <div class="bg-slate-50 pb-12">
                <div class="budget-section grid grid-cols-12 gap-4">
                    <div class="headline px-4 py-10 col-start-2 col-span-6">
                        <h4 class="text-orange-700 text-1xl font-bold">Envelope
                            <br>
                            Budgeting
                        </h4>
                        <h2 class="text-5xl font-bold text-black">{{ title[0] }}</h2>
                        <p class="text-gray-800 py-10 text-2xl font-bold">{{ summry[0] }}</p>
                    </div>
                </div>
                <div class="grid grid-cols-12 gap-4">
                    <div class="service grid grid-cols-3 gap-4 col-start-2 col-span-full">
                        <div class="individual pr-36 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[0] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[1] }}</h3>
                        </div>
                        <div class="individual pr-36 pt-10 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[1] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[2] }}</h3>
                        </div>
                        <div class="individual pr-36 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[2] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[3] }}</h3>
                        </div>
                        <div class="individual pr-36 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[3] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[4] }}</h3>
                        </div>
                        <div class="individual pr-36 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[4] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[5] }}</h3>
                        </div>
                        <div class="individual pr-36 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[5] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[0] }}</h3>
                        </div>
                        <div class="individual pr-36 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[6] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[6] }}</h3>
                        </div>
                        <div class="individual pr-36 pt-10">
                            <h2 class="text-2xl font-bold text-black">{{ arryObj[7] }}</h2>
                            <h3 class="text-orange-700 text-1xl font-bold">{{ arryObj[8].headline[7] }}</h3>
                        </div>
                    </div>
                </div>
            </div>
            <div class=" ions-magic px-4 py-10 pt-10" :style="`background: url(${image4}) no-repeat;`">
                <div class="flex flex-row">
                    <div class="basis-2/4">
                        <img :src="image3" alt="">
                    </div>
                    <div class="basis-2/4">
                        <div class="headline px-4 py-10 col-start-2 col-span-6">
                            <h4 class="text-orange-700 text-1xl font-bold">iOS Magic</h4>
                            <h2 class="text-5xl font-bold text-black">{{ title[1] }}</h2>
                            <p class="text-gray-800 py-10 text-2xl font-bold">{{ summry[1] }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </main>
    </section>
</template>

<style scoped></style>
