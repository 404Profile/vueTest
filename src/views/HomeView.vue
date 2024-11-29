<script setup>
import FooterLink from "@/components/FooterLink.vue";
import HeadPage from "@/components/HeadPage.vue";
import TopFeature from "@/components/TopFeature.vue";
import FeatureCard from "@/components/FeatureCard.vue";
import Features from "@/components/Features.vue";
</script>

<template>
  <div class="antialiased text-slate-400 bg-slate-900">
    <head-page />

    <div>
      <section class="flex w-full">
        <div class="w-1/2 flex items-center justify-center">
          <div class="w-3/4">
            <h1 class="capitalize text-white text-5xl font-semibold">
              <span class="block">Discover your dream</span> property <span class="lowercase">with</span> Estatein
            </h1>

            <div class="pt-5">
              <p>Your journey to finding the perfect property begins here. Explore our listings to find the home that matches your dreams.</p>
            </div>

            <div class="pt-8 flex space-x-4">
              <button class="border border-gray-700 bg-gray-900 px-4 py-3 rounded-lg hover:scale-105">
                <span class="text-white">Learn More</span>
              </button>

              <button class="border border-gray-700 bg-indigo-500 px-4 py-3 rounded-lg relative hover:scale-105">
                <span class="animate-ping absolute inline-flex h-2 w-2 rounded-full bg-sky-400 opacity-75 -top-1 -right-1"></span>
                <span class="text-white">Browse Properities</span>
              </button>
            </div>

            <div class="pt-8 flex space-x-5">
              <div class="bg-gray-800 p-4 rounded-lg border border-gray-700">
                <p class="text-white text-2xl font-bold">200+</p>
                <p>Happy Customers</p>
              </div>

              <div class="bg-gray-800 p-4 rounded-lg border border-gray-700">
                <p class="text-white text-2xl font-bold">10k+</p>
                <p>Properties For CLients</p>
              </div>

              <div class="bg-gray-800 p-4 rounded-lg border border-gray-700">
                <p class="text-white text-2xl font-bold">16+</p>
                <p>Years of Experience</p>
              </div>
            </div>
          </div>
        </div>

        <div class="w-1/2 mt-10 bg-gray-800">
          <img src="" alt="404" class="min-h-[600px]">
        </div>
      </section>

      <section>
        <div class="bg-gray-800 py-3">
          <div class="bg-slate-900 flex justify-between space-x-3 p-3">
            <top-feature text="Find Your Dream Home" />
            <top-feature text="Unlock Property Value" />
            <top-feature text="Effortless Property Management" />
            <top-feature text="Smart Investments, Informed Decisions" />
          </div>
        </div>
      </section>

      <section class="mt-52 max-w-7xl mx-auto">
        <div>
          <div>
            <h2 class="text-white text-4xl font-semibold">Feature Prperties</h2>
          </div>

          <div class="flex justify-between">
            <div class="w-9/12">
              <p>Explore our handpicked selection of featured properties. Each listing offers a glimpse into exceptional homes and investments available through Estate in. Click "View Details" for more information.</p>
            </div>
            <div>
              <button class="border border-gray-700 bg-gray-800 px-4 py-3 rounded-lg hover:scale-105 transition delay-100 duration-500 ease-in-out">
                <span class="text-white">View All Properties</span>
              </button>
            </div>
          </div>
        </div>

        <div class="flex-row space-y-4 sm:mx-0 mx-4 sm:flex sm:space-x-5 sm:space-y-0 mt-20">
          <features />
        </div>
      </section>

      <section class="my-36 max-w-7xl mx-auto">
        <div class="flex justify-between items-center">
          <div>
            <h2 class="text-white text-4xl font-semibold">What Our Clients Say</h2>
            <div class="w-9/12">
              <p>Read the success stories and heartfelt testimonials from our valued clients. Discover why they chose Estatein for their real estate needs.</p>
            </div>
          </div>

          <div>
            <button class="border border-gray-700 bg-gray-800 px-4 py-3 rounded-lg hover:scale-105 transition delay-100 duration-500 ease-in-out">
              <span class="text-white">View All Testimonials</span>
            </button>
          </div>
        </div>

        <div class="max-w-7xl mx-auto">
          <div class="flex-row space-y-4 sm:mx-0 mx-4 sm:flex sm:space-x-5 sm:space-y-0 mt-20">
            <article class="w-full sm:w-1/3">
              <div class="p-4 border border-gray-700 rounded-lg">
                <div>
                  <div>
                    <h3 class="text-white text-2xl font-medium">
                      Exceprional Service!
                    </h3>

                    <p class="pt-2 text-white">
                      Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.
                    </p>
                  </div>

                  <div class="flex space-x-3 mt-4">
                    <div class="h-12 w-12 rounded-full bg-gray-500"></div>

                    <div>
                      <p class="text-white">EWade Warren</p>
                      <p>USA, California</p>
                    </div>
                  </div>
                </div>
              </div>
            </article>

            <article class="w-full sm:w-1/3">
              <div class="p-4 border border-gray-700 rounded-lg">
                <div>
                  <div>
                    <h3 class="text-white text-2xl font-medium">
                      Efficient and Reliable
                    </h3>

                    <p class="pt-2 text-white">
                      Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.
                    </p>
                  </div>

                  <div class="flex space-x-3 mt-4">
                    <div class="h-12 w-12 rounded-full bg-gray-500"></div>

                    <div>
                      <p class="text-white">EWade Warren</p>
                      <p>USA, California</p>
                    </div>
                  </div>
                </div>
              </div>
            </article>

            <article class="w-full sm:w-1/3">
              <div class="p-4 border border-gray-700 rounded-lg">
                <div>
                  <div>
                    <h3 class="text-white text-2xl font-medium">
                      Trusted Advisors
                    </h3>

                    <p class="pt-2 text-white">
                      Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.
                    </p>
                  </div>

                  <div class="flex space-x-3 mt-4">
                    <div class="h-12 w-12 rounded-full bg-gray-500"></div>

                    <div>
                      <p class="text-white">EWade Warren</p>
                      <p>USA, California</p>
                    </div>
                  </div>
                </div>
              </div>
            </article>
          </div>

          <div class="border-t border-gray-700 mt-10">
            <p class="text-center pt-2">
              <span class="text-white">01</span> of 10
            </p>
          </div>
        </div>
      </section>

      <section class="my-36 max-w-7xl mx-auto">
        <div class="flex justify-between items-center">
          <div class="w-9/12">
            <h2 class="text-white text-4xl font-semibold">Start Your Real Estate Journey Today</h2>
            <div class="pt-4">
              <p>Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
            </div>
          </div>

          <div class="w-3/12 flex justify-end">
            <button class="border border-gray-700 bg-indigo-800 px-4 py-3 rounded-lg hover:scale-105 transition delay-100 duration-500 ease-in-out">
              <span class="text-white">Explore Properties</span>
            </button>
          </div>
        </div>
      </section>
    </div>

    <footer>
      <div class="flex max-w-7xl mx-auto">
        <div class="flex-row w-1/3">
          <div>
            <a href="#" class="text-xl font-bold text-white">LOGO</a>
          </div>

          <div class="py-7">
            <label>
              <input class="border border-gray-700 caret-indigo-500 focus:outline-none rounded-lg bg-gray-800 py-2 px-2 w-11/12 focus:border-gray-500" placeholder="Enter Email...">
            </label>
          </div>
        </div>

        <div class="grid grid-cols-5 gap-4 w-2/3 text-right">
          <div>
            <p>Home</p>
            <div class="text-white flex flex-col space-y-2">
              <footer-link text="Link 1"/>
              <footer-link text="Link 2"/>
              <footer-link text="Link 3"/>
              <footer-link text="Link 4"/>
              <footer-link text="Link 5"/>
            </div>
          </div>

          <div>
            <p>About Us</p>
            <div class="text-white flex flex-col space-y-2">
              <footer-link text="Link 1"/>
              <footer-link text="Link 2"/>
              <footer-link text="Link 3"/>
              <footer-link text="Link 4"/>
              <footer-link text="Link 5"/>
            </div>
          </div>

          <div>
            <p>Properties</p>
            <div class="text-white flex flex-col space-y-2">
              <footer-link text="Link 1"/>
              <footer-link text="Link 2"/>
              <footer-link text="Link 3"/>
              <footer-link text="Link 4"/>
              <footer-link text="Link 5"/>
            </div>
          </div>

          <div>
            <p>Services</p>
            <div class="text-white flex flex-col space-y-2">
              <footer-link text="Link 1"/>
              <footer-link text="Link 2"/>
              <footer-link text="Link 3"/>
              <footer-link text="Link 4"/>
              <footer-link text="Link 5"/>
            </div>
          </div>

          <div>
            <p>Contact Us</p>
            <div class="text-white flex flex-col space-y-2">
              <footer-link text="Link 1"/>
              <footer-link text="Link 2"/>
              <footer-link text="Link 3"/>
              <footer-link text="Link 4"/>
              <footer-link text="Link 5"/>
            </div>
          </div>
        </div>
      </div>

      <div class="flex justify-center text-white space-x-10 text-sm py-4 mt-12 bg-gray-800">
        <p>
          @2024 Estatein. All Rights Reserved.
        </p>

        <RouterLink to="#">
          Terms & Conditions
        </RouterLink>
      </div>
    </footer>
  </div>
</template>
