<template>
  <div class="w-full h-[300px]">
    <div>
      <ul>
        <li class="flex justify-center items-center space-x-10 py-[50px]">
          <a href="#" v-for="item in menuItems" :key="item.id" class="">{{
            item.lable
          }}</a>
        </li>
      </ul>
    </div>

    <!-- search button -->
    <div class="flex justify-center items-center">
      <input
        class="w-[929px] h-[56px] border rounded-l-xl pl-3"
        type="text"
        placeholder="Enter your request ..."
      />
      <button
        class="w-[231px] h-[56px] bg-[#B2145B] border rounded-r-xl flex justify-center items-center space-x-3"
      >
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M21 21L16.514 16.506L21 21ZM19 10.5C19 12.7543 18.1045 14.9163 16.5104 16.5104C14.9163 18.1045 12.7543 19 10.5 19C8.24566 19 6.08365 18.1045 4.48959 16.5104C2.89553 14.9163 2 12.7543 2 10.5C2 8.24566 2.89553 6.08365 4.48959 4.48959C6.08365 2.89553 8.24566 2 10.5 2C12.7543 2 14.9163 2.89553 16.5104 4.48959C18.1045 6.08365 19 8.24566 19 10.5V10.5Z"
            stroke="white"
            stroke-width="2"
            stroke-linecap="round"
          />
        </svg>
        <p>Search on the site</p>
      </button>
    </div>

    <!-- language -->
    <div class="flex justify-center items-center space-x-4 pt-[56px] pb-[30px]">
      <span
        ><svg
          width="40"
          height="40"
          viewBox="0 0 40 40"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cx="20" cy="20" r="20" fill="#FAF5EE" />
          <g clip-path="url(#clip0_40_4860)">
            <path
              d="M10 16H30M20 31C26.075 31 31 26.075 31 20C31 13.925 26.075 9 20 9C13.925 9 9 13.925 9 20C9 26.075 13.925 31 20 31ZM20 31C23 31 24 26 24 20C24 14 23 9 20 9C17 9 16 14 16 20C16 26 17 31 20 31ZM10 24H30H10Z"
              stroke="#262626"
              stroke-width="2"
            />
          </g>
          <defs>
            <clipPath id="clip0_40_4860">
              <rect
                width="24"
                height="24"
                fill="white"
                transform="translate(8 8)"
              />
            </clipPath>
          </defs>
        </svg>
      </span>
      <a href="#">ENGLISH</a>
      <a href="#">SPANISH</a>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const menuItems = ref([
  { id: 1, lable: "Home" },
  { id: 2, lable: "Destination" },
  { id: 3, lable: "Tours" },
  { id: 4, lable: "Contact us" },
  { id: 5, lable: "About us" },
]);
</script>

<style lang="scss" scoped></style>
