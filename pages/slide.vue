<template>
  <div>
    <div class="relative w-full p-5">
      <img
        src="/bg.svg"
        class="absolute top-0 left-0 object-cover w-full h-full"
      />
      <div class="w-full mx-auto max-w-7xl">
        <div
          v-for="(path, index) in paths"
          :key="index"
          class="grid grid-cols-2"
        >
          <div class="relative w-full pr-20 h-max">
            <div class="relative p-4">
              <div
                class="border min-h-[200px] rounded-lg flex flex-col justify-center text-white p-5"
              >
                <p class="text-lg font-medium text-center">
                  {{ path[0].month }}
                </p>
                <h1 class="my-3 text-3xl font-bold">
                  {{ path[0].title }}
                </h1>
                <p class="text-white/80">
                  {{ path[0].description }}
                </p>
              </div>
              <img
                src="./assets/golden_border.png"
                class="absolute top-0 right-0 h-full"
                alt=""
              />
            </div>

            <div
              class="h-1 w-[80px] bg-white absolute top-1/2 -translate-y-1/2 right-0 z-[50]"
            >
              <div
                class="absolute w-10 h-10 -translate-y-1/2 bg-white rounded-full left-full top-1/2 ml-[-20px]"
              ></div>
            </div>

            <div
              v-if="index != 0"
              class="absolute right-[-2px] w-1 bg-white h-full top-0"
            ></div>
            <div
              v-else
              class="absolute right-[-2px] w-1 bg-white h-1/2 top-1/2"
            ></div>
          </div>

          <div class="relative w-full pl-20 mt-32 h-max">
            <div class="relative p-4">
              <div
                class="border min-h-[200px] rounded-lg flex flex-col justify-center text-white p-5"
              >
                <p class="text-lg font-medium text-center">
                  {{ path[1].month }}
                </p>
                <h1 class="my-3 text-3xl font-bold">
                  {{ path[1].title }}
                </h1>
                <p class="text-white/80">
                  {{ path[1].description }}
                </p>
              </div>
              <img
                src="./sassets/golden_border.png"
                class="absolute top-0 left-0 h-full rotate-180"
                alt=""
              />
            </div>

            <div
              class="h-1 w-[80px] bg-white absolute top-1/2 -translate-y-1/2 left-0 z-[50]"
            >
              <div
                class="absolute w-10 h-10 -translate-y-1/2 bg-yellow-700 rounded-full right-full top-1/2 mr-[-20px]"
              ></div>
            </div>

            <div
              v-if="index !== paths.length - 1"
              class="absolute w-1 bg-white h-1/2 top-1/2 left-[-2px]"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      paths: [
        [
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
        ],
        [
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
        ],
        [
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
        ],
        [
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
          {
            month: "January",
            title: "Brief",
            description:
              "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus, veniam ex ea cumque incidunt eius dolorum eum, porro eaque nobis labore voluptate minima consequatur velit et commodi suscipit temporibus molestias.",
          },
        ],
      ],
    };
  },
};
</script>
