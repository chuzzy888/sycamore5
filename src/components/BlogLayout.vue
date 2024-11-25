<script>
export default {
  data() {
    return {
      allBlogs: [
        {
          date: "Alec Whitten • 17 Jan 2022",
          title: "Bill Walsh leadership lessons",
          description:
            "Like to know the secrets of transforming a 2-14 team into a 3x Super Bowl winning Dynasty?",
          image: "blg1.png",
          categories: [
            {
              name: "Leadership",
              bgColor: "bg-[#F9F5FF]",
              textColor: "text-[#6941C6]",
            },
            {
              name: "Management",
              bgColor: "bg-[#F8F9FC]",
              textColor: "text-[#363F72]",
            },
          ],
        },
        {
          date: "Demi WIlkinson • 16 Jan 2022",
          title: "PM mental models",
          description:
            "Mental models are simple expressions of complex processes or relationships.",
          image: "blg5.png",
          categories: [
            {
              name: "Product",
              bgColor: "bg-[#F0F9FF]",
              textColor: "text-[#026AA2]",
            },
            {
              name: "Research",
              bgColor: "bg-[#EEF4FF]",
              textColor: "text-[#3538CD]",
            },
            {
              name: "Frameworks",
              bgColor: "bg-[#FFF6ED]",
              textColor: "text-[#C4320A]",
            },
          ],
        },
        {
          date: "Candice Wu • 15 Jan 2022",
          title: "What is Wireframing?",
          description:
            "Introduction to Wireframing and its Principles. Learn from the best in the industry.",
          image: "blg6.png",
          categories: [
            {
              name: "Design",
              bgColor: "bg-[#F9F5FF]",
              textColor: "text-[#6941C6]",
            },
            {
              name: "Research",
              bgColor: "bg-[#EEF4FF]",
              textColor: "text-[#3538CD]",
            },
          ],
        },
        {
          date: "Natali Craig • 14 Jan 2022",
          title: "How collaboration makes us better designers",
          description:
            "Collaboration can make our teams stronger, and our individual designs better.",
          image: "blg7.png",
          categories: [
            {
              name: "Design",
              bgColor: "bg-[#F9F5FF]",
              textColor: "text-[#6941C6]",
            },
            {
              name: "Research",
              bgColor: "bg-[#EEF4FF]",
              textColor: "text-[#3538CD]",
            },
          ],
        },
        {
          date: "Drew Cano • 13 Jan 2022",
          title: "Our top 10 Javascript frameworks to use",
          description:
            "JavaScript frameworks make development easy with extensive features and functionalities.",
          image: "blg8.png",
          categories: [
            {
              name: "Software Development",
              bgColor: "bg-[#ECFDF3]",
              textColor: "text-[#027A48]",
            },
            {
              name: "Tools",
              bgColor: "bg-[#FDF2FA]",
              textColor: "text-[#C11574]",
            },
            {
              name: "SaaS",
              bgColor: "bg-[#FFF1F3]",
              textColor: "text-[#C01048]",
            },
          ],
        },
        {
          date: "Orlando Diggs • 12 Jan 2022",
          title: "Podcast: Creating a better CX Community",
          description:
            "Starting a community doesn’t need to be complicated, but how do you get started?",
          image: "blg9.png",
          categories: [
            {
              name: "Podcasts",
              bgColor: "bg-[#F9F5FF]",
              textColor: "text-[#6941C6]",
            },
            {
              name: "Customer Success",
              bgColor: "bg-[#F8F9FC]",
              textColor: "text-[#363F72]",
            },
          ],
        },
      ],
    };
  },
  methods: {
    getImageUrl(imageName) {
      return new URL(`../assets/images/${imageName}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="bg-white px-6 md:px-16 lg:px-24 py-8">
    <section class="text-center mb-12">
      <p class="text-[#7F56D9] font-semibold">Our blog</p>
      <h1 class="text-4xl font-bold mb-4">Stories and interviews</h1>
      <p class="text-[#667085] max-w-xl mx-auto font-normal">
        Subscribe to learn about new product features, the latest in technology,
        solutions, and updates.
      </p>
      <div class="mt-6 flex justify-center gap-5 flex-col md:flex-row">
        <div class="">
          <input
            type="email"
            placeholder="Enter your email"
            class="border border-gray-300 p-2 rounded-lg d:w-1/3 w-full"
          />
          <p class="text-sm flex gap-1 items-start text-[#667085] mt-2">
            We care about your data in our
            <span class="underline"> privacy policy</span>
          </p>
        </div>
        <div class="">
          <button class="bg-[#7F56D9] text-white p-2 px-3 rounded-lg w-full">
            Subscribe
          </button>
        </div>
      </div>
    </section>

    <section class="mb-12">
      <h2 class="text-2xl font-semibold mb-6 text-[#101828]">
        Recent blog posts
      </h2>
      <div class="flex flex-col md:flex-row gap-8">
        <div class="flex-1 md:w-2/4 relative cursor-pointer">
          <img
            src="@/assets/images/blg2.png"
            alt="Featured Blog"
            class="w-full h-52 2xl:h-80 object-cover"
          />
          <div class="py-4 2xl:py-10">
            <p class="text-[#6941C6]">Olivia Rhye • 20 Jan 2022</p>
            <div class="flex justify-between items-center">
              <h3 class="text-lg font-bold mb-2">UX review presentations</h3>
              <img
                src="@/assets/images/icn.png"
                alt="icon"
                class="object-cover h-2"
              />
            </div>
            <p class="text-gray-600 mb-4 max-w-lg">
              How do you create compelling presentations that wow your
              colleagues and impress your managers?
            </p>
            <div class="flex space-x-2 md:mt-8">
              <span
                class="text-sm bg-[#F9F5FF] text-[#6941C6] px-2 py-1 rounded-3xl"
                >Design</span
              >
              <span
                class="text-sm bg-[#EEF4FF] text-[#3538CD] px-2 py-1 rounded-3xl"
                >Research</span
              >
              <span
                class="text-sm bg-[#FDF2FA] text-[#C11574] px-2 py-1 rounded-3xl"
                >Presentation</span
              >
            </div>
          </div>
        </div>

        <div class="flex flex-col md:w-2/4 space-y-8">
          <div
            class="flex md:flex-row flex-col items-start md:space-x-4 space-y-4 md:space-y-0 cursor-pointer"
          >
            <img
              src="@/assets/images/blg4.png"
              alt="Blog Image"
              class="w-full md:w-2/4 h-full 2xl:h-60 object-cover flex-shrink-0"
            />
            <div class="flex-1 h-full md:w-2/4">
              <p class="text-[#6941C6] mb-1">Phoenix Baker • 19 Jan 2022</p>
              <h3 class="font-bold text-lg mb-1">Migrating to Linear 101</h3>
              <p class="text-gray-600 text-sm mb-3">
                Linear helps streamline software projects, sprints, tasks, and
                bug tracking. Here’s how to get...
              </p>
              <div class="flex space-x-2 md:mt-8">
                <span
                  class="text-sm bg-[#F0F9FF] text-[#026AA2] px-2 py-1 rounded-3xl"
                  >Design</span
                >
                <span
                  class="text-sm bg-[#FDF2FA] text-[#C11574] px-2 py-1 rounded-3xl"
                  >Research</span
                >
              </div>
            </div>
          </div>

          <div
            class="flex md:flex-row flex-col items-start md:space-x-4 space-y-4 md:space-y-0 cursor-pointer"
          >
            <img
              src="@/assets/images/blg3.png"
              alt="Blog Image"
              class="w-full md:w-2/4 h-full 2xl:h-60 object-cover flex-shrink-0"
            />
            <div class="flex-1 h-full md:w-2/4">
              <p class="text-[#6941C6]">Lana Steiner • 18 Jan 2022</p>
              <h3 class="font-bold text-lg mb-1">Building your API Stack</h3>
              <p class="text-gray-600 text-sm mb-3">
                The rise of RESTful APIs has been met by a rise in tools for
                creating, testing, and manag...
              </p>
              <div class="flex space-x-2 md:mt-8">
                <span
                  class="text-sm bg-[#ECFDF3] text-[#027A48] px-2 py-1 rounded-3xl"
                  >Design</span
                >
                <span
                  class="text-sm bg-[#FDF2FA] text-[#C11574] px-2 py-1 rounded-3xl"
                  >Research</span
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <h2 class="text-2xl font-semibold mb-6 text-[#101828]">All blog posts</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <div
          v-for="(blog, index) in allBlogs"
          :key="index"
          class="cursor-pointer"
        >
          <img
            :src="getImageUrl(blog.image)"
            alt="Blog Image"
            class="w-full h-40 object-cover mb-4"
          />
          <p class="text-[#6941C6]">{{ blog.date }}</p>
          <div class="flex justify-between items-center">
            <h3 class="font-bold text-lg mb-2 text-[#101828]">
              {{ blog.title }}
            </h3>
            <img
              src="@/assets/images/icn.png"
              alt="icon"
              class="object-cover h-2"
            />
          </div>
          <p class="text-[#667085] text-sm">{{ blog.description }}</p>
          <div class="flex flex-wrap gap-2">
            <span
              v-for="(category, catIndex) in blog.categories"
              :key="catIndex"
              :class="`${category.bgColor} ${category.textColor} px-2 py-1 rounded-3xl text-sm mt-5`"
            >
              {{ category.name }}
            </span>
          </div>
        </div>
      </div>
    </section>

    <section class="flex flex-col items-center justify-center py-8">
      <div class="w-full border-t border-gray-200 mb-6"></div>

      <nav class="flex items-center space-x-2">
        <button
          class="px-4 py-2 text-gray-500 hover:text-gray-700 flex items-center"
        >
          <span class="mr-2">&larr;</span> Previous
        </button>

        <div class="md:flex space-x-2 hidden">
          <button
            v-for="page in 10"
            :key="page"
            class="w-10 h-10 flex items-center justify-center rounded-lg"
            :class="{
              'bg-[#F4EBFF] text-[#7F56D9]': page === 1,
              'text-gray-700 hover:bg-gray-100': page !== 1,
            }"
          >
            {{ page }}
          </button>
        </div>

        <button
          class="px-4 py-2 text-gray-500 hover:text-gray-700 flex items-center"
        >
          Next <span class="ml-2">&rarr;</span>
        </button>
      </nav>
    </section>
  </div>
</template>

<style scoped>
.container {
  max-width: 1200px;
  margin-left: auto;
  margin-right: auto;
}
</style>
