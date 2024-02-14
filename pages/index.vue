<template>
  <div class="bg-black max-w-[1600px] mx-auto">
    <!-- Navbar -->
    <section>
      <div
        class="h-20 w-full flex items-center justify-around bg-[#191919] text-white"
      >
        <div>LogoHere</div>
        <div class="lg:hidden">
          <i @click="hamburger()" class="fa-solid fa-bars"></i>
        </div>
        <div class="hidden lg:flex items-center gap-28">
          <ul class="flex items-center gap-4 text-nowrap cursor-pointer">
            <li>About</li>
            <li>Collection</li>
            <li>Creater</li>
            <li>Road Map</li>
          </ul>
          <button
            class="bg-[#da904f] hover:transition h-10 w-full p-3 rounded-lg flex items-center justify-center border-2 border-white hover:scale-110 hover:bg-orange-700 hover:ease-in-out duration-300 delay-100"
          >
            Sign in
          </button>
        </div>
      </div>
      <div v-if="isClick">
        <div
          class="fixed top-0 left-0 bg-white h-screen transition ease-in-out duration-300 delay-150 z-[50]"
          :class="{
            'w-[300px] ': !isClick,
            '-w-full': isClick,
          }"
        >
          <div class="flex items-center justify-between gap-5 p-10">
            <div class="text-black text-2xl">Logo</div>
            <div>
              <i
                @click="isClick = !isClick"
                class="fa-solid fa-x text-black"
              ></i>
            </div>
          </div>
          <div class="text-black grid items-center justify-center gap-10">
            <ul class="grid items-center justify-center text-center gap-5">
              <li>About</li>
              <li>Collection</li>
              <li>Creator</li>
              <li>Road Map</li>
            </ul>
            <button
              class="bg-orange-500 h-fit w-[100px] rounded-lg ring-2 ring-offset-2 ring-black text-white p-3"
            >
              Sign in
            </button>
          </div>
        </div>
      </div>
    </section>
    <!-- Navbar -->
    <!-- slide  1-->
    <section>
      <div class="">
        <div class="bg-[url('/bg.svg')]    ">
          <!-- opacity -->
          
          <!-- <img src="./assets/bg.svg" class="w-full" /> -->
          <div class="p-10 md:p-20">
            <div class="md:grid grid-cols-2 gap-10 justify-center items-center">
              <div class="mt-10 text-white">
                <h1 class="text-3xl font-bold xl:text-7xl">
                  We Have High Quality
                  <div
                    class="size-10 flex items-center justify-between gap-20 md:size-20"
                  >
                    <span class="text-[#da904f]">NFT</span>
                    <img src="/filled_star.svg" alt="" />
                  </div>
                  Collections
                </h1>

                <p class="mt-5">
                  Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                  Facere nihil minima libero earum laudantium tempora. Quos
                  dolor asperiores consequatur non necessitatibus aspernatur.
                  Aliquam ipsa accusamus reprehenderit nam veniam enim earum!
                </p>
                <div class="flex items-center gap-10 mt-10">
                  <button
                    class="h-10 w-[150px] p-3 flex items-center justify-center text-nowrap bg-[#da904f] rounded-2xl hover:transition hover:ease-in-out hover:duration-300 delay-10000 hover:scale-110"
                  >
                    Get Whitelist
                  </button>
                  <button
                    class="h-10 w-[150px] p-3 flex items-center justify-center text-nowrap bg-transparent border-2 border-white rounded-2xl  hover:transition hover:ease-in-out hover:duration-300 delay-10000 hover:scale-110"
                  >
                    Contact
                  </button>
                </div>
              </div>
              <div class="mt-10 relative">
                <img src="/tiger_hero.png " />
                <img src="/star.svg" class="size-10" />
                <div
                  class="cursor-pointer text-white absolute right-0 h-20 top-56 border-t-2 border-r-2 border-b-2 p-3 lg:h-56 flex items-center justify-center rounded-e-lg lg:top-64 lg:right-10"
                >
                  <i class="fa-solid fa-chevron-right"></i>
                </div>
              </div>
            </div>
            <div
              class="w-full md:w-[50%] mt-10 text-white flex justify-between bg-white/10 p-5 rounded-xl text-xs md:text-xl"
            >
              <div>
                <h1>240k+</h1>
                <p>Total sale</p>
              </div>
              <div>
                <h1>100k+</h1>
                <p>Auctions</p>
              </div>
              <div>
                <h1>240k+</h1>
                <p>Artists</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- About us slide -->
    <div
      class="text-xl md:h-40 md:text-2xl h-20 bg-black w-full text-white flex items-center justify-center"
    >
      <h1>About us</h1>
    </div>

    <!-- slide 2 -->
    <section>
      <div
        class="bg-[#150e08] w-full p-2 :md:grid items-center justify-between gap-5 lg:gap-10 lg:py-3 md:grid grid-cols-2 px-5"
      >
        <div
          class="flex flex-col gap-5 md:grid grid-cols-2 w-full md:gap-10 xl:p-3"
        >
          <img
            src="/image 104.png"
            alt=""
            class="h-[200px] w-[400px] bg-[#232220] px-3 rounded-lg"
          />
          <img
            src="/image 105.png"
            alt=""
            class="h-[200px] w-[400px] bg-[#232220] px-3 rounded-lg"
          />
          <img
            src="/image 106.png"
            alt=""
            class="h-[200px] w-[400px] bg-[#232220] px-3 rounded-lg"
          />
          <img
            src="/image 107.png"
            alt=""
            class="h-[200px] w-[400px] bg-[#232220] px-3 rounded-lg"
          />
        </div>
        <div
          class="text-white tracking-tighter mt-10 md:text-white flex flex-col items-center justify-center"
        >
          <div>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus
              omnis placeat, natus et quisquam iusto asperiores magni tempora
              alias officia? Obcaecati officiis maxime delectus sint deleniti
              beatae dicta et facere. Lorem ipsum dolor sit amet consectetur,
              adipisicing elit. Excepturi minus error maiores iure voluptas
              molestias aperiam beatae aut, quos fugiat exercitationem, tempore
              ad? Mollitia esse in ex debitis cupiditate quibusdam. Lorem, ipsum
              dolor sit amet consectetur adipisicing elit. Amet tempora quisquam
              magni est, velit nostrum sint odit. Dicta autem corrupti
              veritatis, assumenda architecto rem, vero recusandae est sit
              provident eum.
            </p>
            <p class="mt-2">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Soluta
              illo ipsam omnis veritatis autem repellendus placeat consequuntur
              nisi minima ut.
            </p>
          </div>
          <button
            class="mt-10 bg-white/20 h-fit w-fit p-3 rounded-xl border-orange-400 border-2  hover:transition hover:ease-in-out hover:duration-300 delay-10000 hover:scale-110"
          >
            Connect Wallet
          </button>
        </div>
      </div>
    </section>
    <!-- top collections -->
    <div
      class="bg-black h-48 w-full text-white flex items-center justify-center relative"
    >
      <div
        class="absolute bottom-0 left-0 bg-white rounded-t-full rounded-b-none h-10 w-20 blur-3xl"
      ></div>

      <div>
        <h1
          class="text-2xl flex items-center justify-center md:text-5xl font-bold"
        >
          Top Collections
        </h1>
        <p class="text-center md:leading-normal mt-5">
          The largest and unique Super rare NFT marketplace
          <span class="flex items-center justify-center mt-3"
            >For crypto-collectibles span</span
          >
        </p>
      </div>
    </div>
    <!-- slide 3 -->
    <section>
      <div class="bg-[url('/bg.svg')] h-full w-full p-5">
        <!-- <img src="/bg.svg" class="h-full" /> -->
        <div class="lg:w-full mx-auto xl:w-full max-w-6xl">
          <div
            class="px-3 w-full text-white grid grid-cols-2 md:grid scale-90 md:grid-cols-2 md:px-5 gap-3 justify-center items mt-10 lg:grid-cols-3"
          >
            <div class="bg-white/5 border-orange-500 border p-3 rounded-lg">
              <p>Created by</p>
              <div class="flex items-start justify-start">
                <div class="flex items-center justify-center gap-2">
                  <div class="rounded-full bg-white h-4 w-4"></div>
                  <p class="text-orange-500">James Watson</p>
                </div>
              </div>
              <div>
                <img src="/Frame 1261152802.png" class="mb-3" />
                <h1 class="text-xl font-extrabold">Nfts Collections</h1>

                <p class="text-gray-500">
                  Created by <span class="text-orange-500">James Watson</span>
                </p>
              </div>
            </div>
            <div class="bg-white/5 border-orange-500 border p-3 rounded-lg">
              <p>Created by</p>
              <div class="flex items-start justify-start">
                <div class="flex items-center justify-center gap-2">
                  <div class="rounded-full bg-white h-4 w-4"></div>
                  <p class="text-orange-500">James Watson</p>
                </div>
              </div>
              <div>
                <img src="/Frame 1261152802-1.png" class="mb-3" />
                <p class="text-gray-500">
                  Created by <span class="text-orange-500">James Watson</span>
                </p>
              </div>
            </div>
            <div class="bg-white/5 border-orange-500 border p-3 rounded-lg">
              <p>Created by</p>
              <div class="flex items-start justify-start">
                <div class="flex items-center justify-center gap-2">
                  <div class="rounded-full bg-white h-4 w-4"></div>
                  <p class="text-orange-500">James Watson</p>
                </div>
              </div>
              <div>
                <img src="/Frame 1261152802-1.png" class="mb-3" />
                <p class="text-gray-500">
                  Created by <span class="text-orange-500">James Watson</span>
                </p>
              </div>
            </div>
            <div class="bg-white/5 border-orange-500 border p-3 rounded-lg">
              <p>Created by</p>
              <div class="flex items-start justify-start">
                <div class="flex items-center justify-center gap-2">
                  <div class="rounded-full bg-white h-4 w-4"></div>
                  <p class="text-orange-500">James Watson</p>
                </div>
              </div>
              <div>
                <img src="/Ellipse 130.png" class="mb-3" />
                <p class="text-gray-500">
                  Created by <span class="text-orange-500">James Watson</span>
                </p>
              </div>
            </div>
            <div class="bg-white/5 border-orange-500 border p-3 rounded-lg">
              <p>Created by</p>
              <div class="flex items-start justify-start">
                <div class="flex items-center justify-center gap-2">
                  <div class="rounded-full bg-white h-4 w-4"></div>
                  <p class="text-orange-500">James Watson</p>
                </div>
              </div>
              <div>
                <img src="/Frame 1261152802.png" class="mb-3" />
                <p class="text-gray-500">
                  Created by <span class="text-orange-500">James Watson</span>
                </p>
              </div>
            </div>
            <div class="bg-white/5 border-orange-500 border p-3 rounded-lg">
              <p>Created by</p>
              <div class="flex items-start justify-start">
                <div class="flex items-center justify-center gap-2">
                  <div class="rounded-full bg-white h-4 w-4"></div>
                  <p class="text-orange-500">James Watson</p>
                </div>
              </div>
              <div>
                <img src="/Frame 1261152802-1.png" class="mb-3" />
                <h1 class="text-xl font-extrabold">Nfts Collections</h1>
                <p class="text-gray-500">
                  Created by <span class="text-orange-500">James Watson</span>
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="text-white w-full flex items-center justify-center">
          <button
            class="h-fit w-fit p-4 bg-white/10 rounded-xl border border-orange-500  hover:transition hover:ease-in-out hover:duration-300 delay-10000 hover:scale-110"
          >
            Explore More
          </button>
        </div>
      </div>
    </section>
    <!-- slide 4 -->
    <section>
      <div class="h-full w-full bg-black -mt-2 p-5 relative">
        <div
          class="absolute top-0 right-0 bg-white rounded-t-full rounded-b-none h-10 w-20 blur-3xl"
        ></div>

        <div
          class="absolute bottom-0 left-0 bg-white rounded-t-full rounded-b-none h-10 w-20 blur-3xl"
        ></div>

        <div class="text-white mt-20">
          <h1 class="text-center text-3xl font-bold">Top creators</h1>
          <p class="text-center mt-4">
            Checkout Top Rated Creators On The NFT Marketplace
          </p>
        </div>
        <div
          class="grid justify-center items-center mt-5 md:max-w-4xl mx-auto xl:scale-110"
        >
          <div
            class="grid grid-cols-1 md:mt-20 md:grid md:grid-cols-2 gap-3 lg:grid-cols-4"
          >
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 137.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 138.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 136.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 135.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 133.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 134.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 134-1.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
            <div class="h-fit w-[200px] bg-white/10 p-5 rounded-xl">
              <div
                class="h-4 w-4 bg-gray-600 text-white rounded-full flex items-center justify-center text-xs"
              >
                1
              </div>
              <div>
                <img src="/Ellipse 133-1.png" class="scale-75" />
              </div>
              <div class="text-white text-center">
                <h1>Name NFT</h1>
                <p class="font-thin text-xs scale-110">
                  <span class="text-xs text-[#46453f]">Total sales : </span
                  >34.53 ETH
                </p>
              </div>
            </div>
          </div>
        </div>
        <div
          class="text-white mt-20 text-3xl font-bold flex justify-center items-center mb-20"
        >
          <h1>Road Map</h1>
        </div>
      </div>
    </section>
    <!-- slide 5 -->
    <section>
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
              class="grid md:grid-cols-2"
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
                    src="/golden_border.png"
                    class="absolute top-0 right-0 h-full"
                    alt=""
                  />
                </div>

                <div
                  class="md:h-1 w-[80px] md:bg-white absolute top-1/2 -translate-y-1/2 right-0 z-[50]"
                >
                  <div
                    class="md:absolute w-10 h-10 -translate-y-1/2 md:bg-white rounded-full left-full top-1/2 ml-[-20px]"
                  ></div>
                </div>

                <div
                  v-if="index != 0"
                  class="md:absolute right-[-2px] w-1 md:bg-white h-full top-0"
                ></div>
                <div
                  v-else
                  class="absolute right-[-2px] w-1 md:bg-white h-1/2 top-1/2"
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
                    src="/golden_border.png"
                    class="absolute top-0 left-0 h-full rotate-180"
                    alt=""
                  />
                </div>

                <div
                  class="md:h-1 w-[80px] md:bg-white absolute top-1/2 -translate-y-1/2 left-0 z-[50]"
                >
                  <div
                    class="md:absolute w-10 h-10 -translate-y-1/2 md:bg-yellow-700 rounded-full right-full top-1/2 mr-[-20px]"
                  ></div>
                </div>

                <div
                  v-if="index !== paths.length - 1"
                  class="absolute w-1 md:bg-white h-1/2 top-1/2 left-[-2px]"
                ></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- slide 6 -->
    <section>
      <div class="bg-black -mt-5 md:max-w-full mx-auto p-10 relative">
        <div
        class="absolute top-0 right-0 bg-white rounded-t-full rounded-b-none h-10 w-20 blur-3xl"
      ></div>

      <div
        class="absolute bottom-0 left-0 bg-white rounded-t-full rounded-b-none h-10 w-20 blur-3xl"
      ></div>
      <div
      class="absolute bottom-72 right-0 bg-white rounded-t-full rounded-b-none h-10 w-20  blur-3xl"
    ></div>
    <div
    class="absolute bottom-72 left-0 bg-white rounded-t-full rounded-b-none h-10 w-20  blur-3xl md:hidden"
  ></div>

    <div
      class="absolute bottom-0 left-0 bg-white rounded-t-full rounded-b-none h-10 w-20 blur-3xl"
    ></div>
        <div
          class="text-white flex items-center justify-center pt-20 font-bold text-4xl"
        >
          <h1>How it Works</h1>
        </div>
        <div class="grid md:grid-cols-2 items-center justify-center">
          <img src="/wallet.svg" class="" />
          <div class="text-white">
            <img src="/filled_star.svg" alt="" />
            <h1 class="text-5xl font-bold tracking-wider mt-5 lg:px-10">
              Setup And Connect Your Wallet.
            </h1>
            <p class="mt-10 lg:px-10">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos qui
              nam, consectetur soluta ducimus itaque fugit sit tempore? Sequi,
              atque! Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              At, quidem?
            </p>
          </div>
        </div>
        <div
          class="grid md:grid-cols-2 items-center justify-center mt-10 gap-20"
        >
          <div class="text-white">
            <h1 class="text-6xl font-bold mt-5 lg:px-10">
              Create Your Own Digital NFT
            </h1>
            <p class="mt-10 tracking-tighter lg:px-10">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos qui
              nam, consectetur soluta ducimus itaque fugit sit tempore? Sequi,
              atque! Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              At, quidem?
            </p>
          </div>
          <div class="w-fit h-fit bg-gray-600/10 rounded-3xl">
            <img src="/monkey.svg" />
          </div>
        </div>

        <div
          class="grid mt-20 md:grid-cols-2 gap-2 items-center justify-center"
        >
          <div>
            <div class="flex items-end justify-end">
              <img src="/filled_star.svg" class="h-20" />
            </div>
            <div>
              <img src="/goldman.svg" />
            </div>
          </div>
          <div class="text-white">
            <h1 class="text-5xl font-bold tracking-wider mt-5 lg:px-10">
              Setup And Connect Your Wallet.
            </h1>
            <p class="mt-10 lg:px-10">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos qui
              nam, consectetur soluta ducimus itaque fugit sit tempore? Sequi,
              atque! Lorem ipsum dolor, sit amet consectetur adipisicing elit.
              At, quidem?
            </p>
          </div>
        </div>
      </div>
    </section>
    <!-- slide 7 -->
    <section>
      <div class="bg-[url('/bg.svg')] h-full py-5 md:px-20 w-full px-10">
        <div>
          <div class="text-white text-center font-bold text-2xl">
            <h1>Join OurCommunity</h1>
          </div>
          <div
            class="text-white md:tracking-tight md:text-justify mt-10 lg:px-20 xl:px-56"
          >
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptas
              at reiciendis nam quas porro cupiditate non deserunt iure, alias
              accusamus. Enim dolores atque vero nostrum nemo. Dolore eveniet
              eos, eligendi non, sint delectus suscipit consequuntur nam vero,
              rerum error iusto?
            </p>
          </div>
          <div
            class="mt-10 grid md:flex justify-between w-full gap-10 lg:justify-center"
          >
            <input
              type="email"
              placeholder="Your Email"
              class="w-full lg:w-[500px] xl:w-[700px] h-10 rounded-3xl p-5 font-thin"
            />
            <button
              class="text-white h-10 w-fit bg-white/55 p-5 flex justify-center items-center rounded-3xl ring-2 ring-offset-2 ring-orange-400 text-nowrap  hover:transition hover:ease-in-out hover:duration-300 delay-10000 hover:scale-110"
            >
              Join now
            </button>
          </div>
        </div>
        <div class="text-white mt-5 text-center">
          <p>© NFT Market. Use this template freely.</p>
        </div>
      </div>
    </section>
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
      ],
      isClick: false,
    };
  },
  methods: {
    hamburger() {
      this.isClick = !this.isClick;
    },
  },
};
</script>
