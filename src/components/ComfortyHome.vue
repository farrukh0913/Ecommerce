<template>
  <div id="home">
    <div>
      <header class="font-display">
        <div id="header-sticky" class="">

          <div class="main-header bg-grayscales-500 lg:border-none border-b border-grayscales-700">
            <div class="container px-3 md:px-5 xl:px-0">
              <div class="flex justify-between items-center py-5" id="responsive-nav">
                <div>
                  <a href="index.html">
                    <img :src="require('@/assets/images/all-img/logo.png')" alt="">
                  </a>
                </div>
                <div class="lg:max-w-[413px] lg:block " id="search-input">
                  <div class="relative">
                    <input type="text" id="search" placeholder="search here..."
                      class="block w-full bg-white focus:outline-none border-0 px-4 py-3 rounded-lg focus:ring-2 ring-[#029FAE]">
                    <label for="search" class="absolute right-4 top-3">
                      <svg width="23" height="22" viewBox="0 0 23 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                          d="M10.5833 17.4167C14.6334 17.4167 17.9167 14.1334 17.9167 10.0833C17.9167 6.03325 14.6334 2.75 10.5833 2.75C6.53325 2.75 3.25 6.03325 3.25 10.0833C3.25 14.1334 6.53325 17.4167 10.5833 17.4167Z"
                          stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                        <path d="M19.75 19.25L15.7625 15.2625" stroke="#272343" stroke-width="1.5"
                          stroke-linecap="round" stroke-linejoin="round" />
                      </svg>
                    </label>
                  </div>
                </div>
                <div class="lg:block ">
                  <ul class="flex items-center gap-3">
                    <li class="relative">
                      <a href="#" class="inline-flex gap-2 bg-white rounded-lg p-[11px]" id="addToCart">
                        <span><svg width="22" height="22" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52087 2.97916L4.42754 3.30916L5.31029 13.8261C5.3442 14.2399 5.5329 14.6258 5.83873 14.9066C6.14457 15.1875 6.54506 15.3427 6.96029 15.3413H16.9611C17.3587 15.3418 17.7431 15.1986 18.0436 14.9383C18.344 14.6779 18.5404 14.3178 18.5965 13.9242L19.4673 7.91266C19.4905 7.75279 19.482 7.58991 19.4422 7.43333C19.4024 7.27675 19.3322 7.12955 19.2354 7.00015C19.1387 6.87074 19.0175 6.76167 18.8786 6.67917C18.7397 6.59667 18.5859 6.54235 18.426 6.51933C18.3673 6.51291 4.73371 6.50833 4.73371 6.50833"
                              stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.948 9.89542H15.4899" stroke="#272343" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.55786 18.5194C6.62508 18.5165 6.69219 18.5273 6.75515 18.551C6.81811 18.5748 6.87562 18.611 6.9242 18.6575C6.97279 18.7041 7.01145 18.76 7.03787 18.8219C7.06428 18.8837 7.0779 18.9503 7.0779 19.0176C7.0779 19.0849 7.06428 19.1515 7.03787 19.2134C7.01145 19.2753 6.97279 19.3312 6.9242 19.3777C6.87562 19.4243 6.81811 19.4605 6.75515 19.4842C6.69219 19.508 6.62508 19.5187 6.55786 19.5158C6.42942 19.5103 6.30808 19.4554 6.21914 19.3626C6.13021 19.2698 6.08057 19.1462 6.08057 19.0176C6.08057 18.8891 6.13021 18.7655 6.21914 18.6726C6.30808 18.5798 6.42942 18.5249 6.55786 18.5194Z"
                              fill="#272343" stroke="#272343" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.5721 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.5721 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="#272343" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </span>
                        <span>Cart</span>
                        <span
                          class="bg-dark-accents text-white rounded-full py-[3px] px-[9px] ml-1 inline-flex justify-center items-center text-[10px] leading-[100%]">2</span>
                      </a>
                      <div class="cart-content">
                        <ul class="p-6">
                          <li class="pb-4">
                            <div class="flex items-center justify-between">
                              <div class="flex items-center gap-1">
                                <div>
                                  <img :src="require('@/assets/images/all-img/cart-01.png')" alt="">
                                </div>
                                <div class="px-2">
                                  <h2 class="text-gray-black"><span>Isolate Sofa Chair</span> <span
                                      class="text-[#636270]">x5</span></h2>
                                  <p class="text-gray-black font-semibold mb-0">$150.00</p>
                                </div>
                              </div>
                              <div>
                                <button
                                  class="hover:bg-[#F0F2F3] bg-transparent p-2 hover:text-gray-black rounded-full text-[#9A9CAA] transition-all duration-500">
                                  <svg width="28" height="28" viewBox="0 0 28 28" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path d="M10 10L14 14M14 14L18 10M14 14L10 18M14 14L18 18" stroke="currentColor"
                                      stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                                  </svg>
                                </button>
                              </div>
                            </div>
                          </li>
                          <li class="py-4">
                            <div class="flex items-center justify-between">
                              <div class="flex items-center gap-1">
                                <div>
                                  <img :src="require('@/assets/images/all-img/cart-01.png')" alt="">
                                </div>
                                <div class="px-2">
                                  <h2 class="text-gray-black"><span>Isolate Sofa Chair</span> <span
                                      class="text-[#636270]">x5</span></h2>
                                  <p class="text-gray-black font-semibold mb-0">$150.00</p>
                                </div>
                              </div>
                              <div>
                                <button
                                  class="hover:bg-[#F0F2F3] bg-transparent p-2 hover:text-gray-black rounded-full text-[#9A9CAA] transition-all duration-500">
                                  <svg width="28" height="28" viewBox="0 0 28 28" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path d="M10 10L14 14M14 14L18 10M14 14L10 18M14 14L18 18" stroke="currentColor"
                                      stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                                  </svg>
                                </button>
                              </div>
                            </div>
                          </li>
                          <div class="flex justify-between items-center py-2 mb-4">
                            <p class="text-[#636270] text-lg">2 Products</p>
                            <p class="text-gray-black text-xl font-medium">$250.00</p>
                          </div>
                          <div class="flex justify-between items-center">
                            <a href="shopping-cart.html" class="btn-transparent">View Cart</a>
                            <a href="checkout-shopping.html" class="btn-primary">Checkout</a>
                          </div>
                        </ul>
                      </div>
                    </li>
                    <li class="inline-flex items-center justify-center">
                      <a href="#" class="bg-white text-gray-black hover:text-[#007580] rounded-lg p-[11px]">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M2.63262 10.6315C1.64903 7.56067 2.79762 4.05075 6.02245 3.01217C6.85867 2.74459 7.74676 2.68086 8.61262 2.82629C9.47849 2.97172 10.297 3.32208 10.9999 3.84817C12.3337 2.81692 14.2743 2.46858 15.9683 3.01217C19.1922 4.05075 20.349 7.56067 19.3664 10.6315C17.8355 15.499 10.9999 19.2482 10.9999 19.2482C10.9999 19.2482 4.21478 15.5558 2.63262 10.6315V10.6315Z"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                      </a>
                    </li>
                    <li class="relative">
                      <button class="bg-white text-gray-black hover:text-[#007580] rounded-lg p-[11px] user-profile">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M10.9862 14.0672C7.44053 14.0672 4.4137 14.6034 4.4137 16.7503C4.4137 18.8971 7.42128 19.4526 10.9862 19.4526C14.5309 19.4526 17.5587 18.9154 17.5587 16.7695C17.5587 14.6236 14.5502 14.0672 10.9862 14.0672V14.0672Z"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M10.9862 11.0055C11.8195 11.0055 12.634 10.7584 13.3268 10.2955C14.0197 9.83255 14.5597 9.17457 14.8785 8.40475C15.1974 7.63492 15.2808 6.78783 15.1183 5.97058C14.9557 5.15334 14.5545 4.40266 13.9653 3.81346C13.3761 3.22426 12.6254 2.82301 11.8081 2.66045C10.9909 2.49789 10.1438 2.58132 9.37397 2.9002C8.60415 3.21907 7.94617 3.75906 7.48324 4.45188C7.02031 5.14471 6.77322 5.95925 6.77322 6.7925C6.76932 7.90581 7.20779 8.97508 7.99218 9.76515C8.77657 10.5552 9.84266 11.0014 10.956 11.0055H10.9862Z"
                            stroke="currentColor" stroke-width="1.429" stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                      </button>
                      <div class="profile-content">
                        <ul class="py-3" id="cart-dropdown" style="display:none">
                          <div class="px-3 shadow-[0px_1px_0px_#E1E3E6]">
                            <li>
                              <a href="sign-in.html">Sign In</a>
                            </li>
                            <li>
                              <a href="sign-up.html">Create a Account</a>
                            </li>
                          </div>
                          <div class="px-3 shadow-[0px_1px_0px_#E1E3E6]">
                            <li>
                              <a href="account-setting.html">Account Settings</a>
                            </li>
                            <li>
                              <a href="order-history.html">Order History</a>
                            </li>
                          </div>
                          <div class="px-3 shadow-[0px_1px_0px_#E1E3E6]">
                            <li>
                              <a href="wishlist.html">Wishlist</a>
                            </li>
                            <li>
                              <a href="shopping-cart.html">Shopping Cart</a>
                            </li>
                          </div>
                          <div class="px-3">
                            <li>
                              <a href="#">Logout</a>
                            </li>
                          </div>
                        </ul>
                      </div>
                    </li>
                  </ul>
                </div>
                <div class="lg:hidden inline-block hamburger-btn" id="hamburger-btn">
                  <span></span>
                  <span></span>
                  <span></span>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="bottom-header bg-white shadow-[0px_1px_0px_#E1E3E6] relative z-30  lg:block">
          <div class="container px-3 md:px-5 xl:px-0">
            <div class="py-3.5 flex justify-between items-center">
              <div class="flex gap-8 items-center">
                <div class="relative">
                  <button
                  
                    class="max-h-12 inline-flex items-center justify-center gap-4 py-3.5 px-5 border border-grayscales-700 rounded-md custom-dropdown text-gray-black text-sm leading-4 font-medium font-display">
                    <span class="text-gray-black inline-flex">
                      <svg width="18" height="14" viewBox="0 0 18 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M18 2.5H0V0.5H18V2.5Z" fill="currentColor" />
                        <path d="M18 8.5H0V6.5H18V8.5Z" fill="currentColor" />
                        <path d="M18 14.5H0V12.5H18V14.5Z" fill="currentColor" />
                      </svg>
                    </span>
                    <span class="text-gray-black inline-flex">All Categories</span>
                  </button>
                 
                </div>

                <ul class="lg:flex gap-8 items-center hidden main-menu" id="dropdown-for-sub-header">
                  <li>
                    <a href="index.html">Home</a>
                  </li>
                  <li>
                    <a href="products.html">Shop</a>
                  </li>
                  <li>
                    <a href="product-details.html">Product</a>
                  </li>
                  <li class="relative">
                    <a href="javascript:void(0);" class="inline-flex gap-2 items-center">Pages
                      <span>
                        <img :src="require('@/assets/images/all-img/select-arrow.png')" alt="">
                      </span>
                    </a>
                    <ul id="pages-dropdown-header" style="display: none;">
                      <li>
                        <a href="404.html">404</a>
                      </li>
                      <li>
                        <a href="account-setting.html">Account Setting</a>
                      </li>
                      <li>
                        <a href="sign-in.html">Sign In</a>
                      </li>
                      <li>
                        <a href="sign-up.html">Sign Up</a>
                      </li>
                      <li>
                        <a href="forget-password.html">Forget Password</a>
                      </li>
                      <li>
                        <a href="change-password.html">Change Password</a>
                      </li>
                      <li>
                        <a href="products.html">Product List</a>
                      </li>
                      <li>
                        <a href="product-details.html">Product Details</a>
                      </li>
                      <li>
                        <a href="shopping-cart.html">Shopping Cart</a>
                      </li>
                      <li>
                        <a href="wishlist.html">Wishlist</a>
                      </li>
                      <li>
                        <a href="checkout-billing.html">Checkout Billing</a>
                      </li>
                      <li>
                        <a href="checkout-shopping.html">Checkout Shoping</a>
                      </li>
                    </ul>
                  </li>
                  <li>
                    <a href="">About</a>
                  </li>
                </ul>
              </div>
              <div>
                <p class="text-grayscales-900 inline-flex gap-2 items-center text-sm font-display">
                  <span>Contact:</span><span class="text-secondary font-medium">(808) 555-0111</span></p>
              </div>
            </div>
          </div>
        </div>
        <!-- Mobile Menu Area Start -->
        <div class="nav-menu" id="nav-menu" style="display:none">
          <div class="flex justify-between  items-center px-3 py-4 mb-4">
            <div>
              <a href="#">
                <img :src="require('@/assets/images/all-img/logo-sm.png')" alt="">
              </a>
            </div>
            <ul class="flex items-center gap-3">
              <li>
                <a href="#" class="inline-flex gap-2 bg-white rounded-lg p-[11px] relative">
                  <span>
                    <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path
                        d="M2.52087 2.97916L4.42754 3.30916L5.31029 13.8261C5.3442 14.2399 5.5329 14.6258 5.83873 14.9066C6.14457 15.1875 6.54506 15.3427 6.96029 15.3413H16.9611C17.3587 15.3418 17.7431 15.1986 18.0436 14.9383C18.344 14.6779 18.5404 14.3178 18.5965 13.9242L19.4673 7.91266C19.4905 7.75279 19.482 7.58991 19.4422 7.43333C19.4024 7.27675 19.3322 7.12955 19.2354 7.00015C19.1387 6.87074 19.0175 6.76167 18.8786 6.67917C18.7397 6.59667 18.5859 6.54235 18.426 6.51933C18.3673 6.51291 4.73371 6.50833 4.73371 6.50833"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                      <path d="M12.948 9.89542H15.4899" stroke="#272343" stroke-width="1.5" stroke-linecap="round"
                        stroke-linejoin="round" />
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M6.55786 18.5194C6.62508 18.5165 6.69219 18.5273 6.75515 18.551C6.81811 18.5748 6.87562 18.611 6.9242 18.6575C6.97279 18.7041 7.01145 18.76 7.03787 18.8219C7.06428 18.8837 7.0779 18.9503 7.0779 19.0176C7.0779 19.0849 7.06428 19.1515 7.03787 19.2134C7.01145 19.2753 6.97279 19.3312 6.9242 19.3777C6.87562 19.4243 6.81811 19.4605 6.75515 19.4842C6.69219 19.508 6.62508 19.5187 6.55786 19.5158C6.42942 19.5103 6.30808 19.4554 6.21914 19.3626C6.13021 19.2698 6.08057 19.1462 6.08057 19.0176C6.08057 18.8891 6.13021 18.7655 6.21914 18.6726C6.30808 18.5798 6.42942 18.5249 6.55786 18.5194Z"
                        fill="#272343" stroke="#272343" stroke-width="1.5" stroke-linecap="round"
                        stroke-linejoin="round" />
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.5721 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.5721 16.7663 18.5194 16.8988 18.5194Z"
                        fill="#272343" stroke="#272343" stroke-width="1.5" stroke-linecap="round"
                        stroke-linejoin="round" />
                    </svg>
                  </span>
                  <span
                    class="bg-dark-accents absolute -top-1 right-0 text-white rounded-full px-2 py-1.5 inline-flex justify-center items-center text-[10px] leading-[100%]">2</span>
                </a>
              </li>
              <li>
                <a href="#" class="bg-white text-gray-black flex hover:text-[#007580] rounded-lg p-[11px]">
                  <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd"
                      d="M2.63262 10.6315C1.64903 7.56067 2.79762 4.05075 6.02245 3.01217C6.85867 2.74459 7.74676 2.68086 8.61262 2.82629C9.47849 2.97172 10.297 3.32208 10.9999 3.84817C12.3337 2.81692 14.2743 2.46858 15.9683 3.01217C19.1922 4.05075 20.349 7.56067 19.3664 10.6315C17.8355 15.499 10.9999 19.2482 10.9999 19.2482C10.9999 19.2482 4.21478 15.5558 2.63262 10.6315V10.6315Z"
                      stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                  </svg>
                </a>
              </li>
              <li class="relative">
                <button class="bg-white text-gray-black hover:text-[#007580] rounded-lg p-[11px] user-profile">
                  <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path fill-rule="evenodd" clip-rule="evenodd"
                      d="M10.9862 14.0672C7.44053 14.0672 4.4137 14.6034 4.4137 16.7503C4.4137 18.8971 7.42128 19.4526 10.9862 19.4526C14.5309 19.4526 17.5587 18.9154 17.5587 16.7695C17.5587 14.6236 14.5502 14.0672 10.9862 14.0672V14.0672Z"
                      stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    <path fill-rule="evenodd" clip-rule="evenodd"
                      d="M10.9862 11.0055C11.8195 11.0055 12.634 10.7584 13.3268 10.2955C14.0197 9.83255 14.5597 9.17457 14.8785 8.40475C15.1974 7.63492 15.2808 6.78783 15.1183 5.97058C14.9557 5.15334 14.5545 4.40266 13.9653 3.81346C13.3761 3.22426 12.6254 2.82301 11.8081 2.66045C10.9909 2.49789 10.1438 2.58132 9.37397 2.9002C8.60415 3.21907 7.94617 3.75906 7.48324 4.45188C7.02031 5.14471 6.77322 5.95925 6.77322 6.7925C6.76932 7.90581 7.20779 8.97508 7.99218 9.76515C8.77657 10.5552 9.84266 11.0014 10.956 11.0055H10.9862Z"
                      stroke="currentColor" stroke-width="1.429" stroke-linecap="round" stroke-linejoin="round" />
                  </svg>
                </button>
                <div class="profile-content" style="display:none" id="profile-dropdown">
                  <ul>
                    <li>
                      <a href="#">Wodden</a>
                    </li>
                    <li>
                      <a href="#">Partex</a>
                    </li>
                    <li>
                      <a href="#">Plywood</a>
                    </li>
                    <li>
                      <a href="#">Segun</a>
                    </li>
                  </ul>
                </div>
              </li>
              <li>
                <span
                  class="hamburger-btn-close bg-[#F7F7F9] text-black w-[44px] h-[44px] rounded-full flex items-center justify-center"
                  id="hamburger-btn-close">
                  <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M11 1L1 11" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                      stroke-linejoin="round"></path>
                    <path d="M1 1L11 11" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                      stroke-linejoin="round"></path>
                  </svg>
                </span>
              </li>
            </ul>
          </div>
          <div class="px-3 mb-4">
            <div class="lg:max-w-[413px] w-full">
              <div class="relative">
                <input type="text" placeholder="search here..."
                  class="block w-full bg-grayscales-500 focus:outline-none border-0 px-4 py-3 rounded-lg">
                <span class="absolute right-4 top-3">
                  <svg width="23" height="22" viewBox="0 0 23 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path
                      d="M10.5833 17.4167C14.6334 17.4167 17.9167 14.1334 17.9167 10.0833C17.9167 6.03325 14.6334 2.75 10.5833 2.75C6.53325 2.75 3.25 6.03325 3.25 10.0833C3.25 14.1334 6.53325 17.4167 10.5833 17.4167Z"
                      stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    <path d="M19.75 19.25L15.7625 15.2625" stroke="#272343" stroke-width="1.5" stroke-linecap="round"
                      stroke-linejoin="round" />
                  </svg>
                </span>
              </div>
            </div>
          </div>
          <!-- menu -->
          <div>
            <nav class="tabs flex flex-row">
              <button data-target="panel-1"
                class="tab rounded-none w-1/2 active text-gray-600 py-4 px-6 block hover:text-blue-500 focus:outline-none text-blue-500 border-b-2 font-medium border-blue-500">
                Menu
              </button>
              <button data-target="panel-2"
                class="tab rounded-none w-1/2 ext-gray-600 py-4 px-6 block hover:text-blue-500 focus:outline-none border-b-2 font-medium border-blue-500">
                Categories
              </button>
            </nav>
          </div>

          <div id="panels">
            <div class="panel-1 tab-content active">
              <ul class="flex flex-col items-center">
                <li class="w-full block">
                  <a href="" class="border-b border-[#029FAE] block px-3 py-2">Home</a>
                </li>
                <li class="w-full block">
                  <a href="" class="border-b border-[#029FAE] block px-3 py-2">Shop</a>
                </li>
                <li class="w-full block">
                  <a href="" class="border-b border-[#029FAE] block px-3 py-2">Product</a>
                </li>
                <li class="w-full block">
                  <a href="" class="border-b border-[#029FAE] block px-3 py-2">Pages</a>
                </li>
                <li class="w-full block">
                  <a href="" class="border-b border-[#029FAE] block px-3 py-2">About</a>
                </li>
              </ul>
            </div>
            <div class="panel-2 tab-content py-5">
              <ul>
                <li>
                  <a href="#" class="border-b border-[#029FAE] block px-3 py-2">Wodden</a>
                </li>
                <li>
                  <a href="#" class="border-b border-[#029FAE] block px-3 py-2">Partex</a>
                </li>
                <li>
                  <a href="#" class="border-b border-[#029FAE] block px-3 py-2">Plywood</a>
                </li>
                <li>
                  <a href="#" class="border-b border-[#029FAE] block px-3 py-2">Segun</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <!-- Mobile Menu Area End -->
        <div class="overlay" id="overlay"></div>
      </header>
      <!-- header area end -->

      <!-- banner section start -->
      <section
        class="banner-section 2xl:mx-[90px] bg-grayscales-500 rounded-bl-[20px] rounded-br-[20px] font-display relative z-10">
        <div class="swiper bannerSwiper xl:pt-20 py-6 xl:pb-28 relative z-50">
          <div class="swiper-wrapper" id="swiper-wrapper">
            <div class="swiper-slide">
              <div class="container px-3 md:px-5 flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 w-full" id="header-content">
                  <p class="text-gray-black text-sm tracking-[0.12em] mb-2">Welcome to Comforty</p>
                  <h1 class="xl:text-[68px] text-xl md:text-3xl xl:leading-[110%] text-gray-black font-semibold mb-6">
                    Best Furniture Collection for your interior.</h1>
                  <div>
                    <a href="#" class="btn-primary">
                      <span id="btn-primary">Shop Now.</span>
                      <span><svg width="24" height="24" viewBox="0 0 24 24" fill="none"
                          xmlns="http://www.w3.org/2000/svg">
                          <path d="M15.5 7.5L20 12M20 12L15.5 16.5M20 12H4" stroke="white" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                      </span>
                    </a>
                  </div>
                </div>
                <div class="md:w-1/2 w-full flex justify-center items-center relative" id='blob'>
                  <img :src="require('@/assets/images/all-img/chair.png')" alt="">
                  <div class="inline-block absolute top-0 right-0">
                    <img :src="require('@/assets/images/all-img/discount.png')" alt="">
                    <p class="absolute top-[33px] text-[#F05C52] text-4xl font-bold right-9">15%</p>
                    <p class="absolute text-sm font-normal top-[68px] right-10">Discount</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="swiper-slide" id="swiper-slide-2">
              <div class="container px-3 md:px-5 flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 w-full">
                  <p class="text-gray-black text-sm tracking-[0.12em] mb-2">Welcome to chairy</p>
                  <h1 class="xl:text-[68px] text-xl md:text-3xl xl:leading-[110%] text-gray-black font-semibold mb-6">
                    Best Furniture Collection for your interior.</h1>
                  <div>
                    <a href="#" class="btn-primary">
                      <span>Shop Now</span>
                      <span><svg width="24" height="24" viewBox="0 0 24 24" fill="none"
                          xmlns="http://www.w3.org/2000/svg">
                          <path d="M15.5 7.5L20 12M20 12L15.5 16.5M20 12H4" stroke="white" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                      </span>
                    </a>
                  </div>
                </div>
                <div class="md:w-1/2 w-full flex justify-center items-center relative">
                  <img :src="require('@/assets/images/all-img/chair.png')" alt="">
                  <div class="inline-block absolute top-0 right-0">
                    <img :src="require('@/assets/images/all-img/discount.png')" alt="">
                    <p class="absolute top-[33px] text-[#F05C52] text-4xl font-bold right-9">15%</p>
                    <p class="absolute text-sm font-normal top-[68px] right-10">Discount</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="swiper-slide" id="swiper-slide-3">
              <div class="container px-3 md:px-5 flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 w-full">
                  <p class="text-gray-black text-sm tracking-[0.12em] mb-2">Welcome to chairy</p>
                  <h1 class="xl:text-[68px] text-xl md:text-3xl xl:leading-[110%] text-gray-black font-semibold mb-6">
                    Best Furniture Collection for your interior.</h1>
                  <div>
                    <a href="#" class="btn-primary">
                      <span>Shop Now</span>
                      <span><svg width="24" height="24" viewBox="0 0 24 24" fill="none"
                          xmlns="http://www.w3.org/2000/svg">
                          <path d="M15.5 7.5L20 12M20 12L15.5 16.5M20 12H4" stroke="white" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                      </span>
                    </a>
                  </div>
                </div>
                <div class="md:w-1/2 w-full flex justify-center items-center relative">
                  <img :src="require('@/assets/images/all-img/chair.png')" alt="">
                  <div class="inline-block absolute top-0 right-0">
                    <img :src="require('@/assets/images/all-img/discount.png')" alt="">
                    <p class="absolute top-[33px] text-[#F05C52] text-4xl font-bold right-9">15%</p>
                    <p class="absolute text-sm font-normal top-[68px] right-10">Discount</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="swiper-button-next banner-slider-button"></div>
          <div class="swiper-button-prev banner-slider-button"></div>
          <div class="swiper-pagination"></div>
        </div>
        <img :src="require('@/assets/images/svg/banner-shapes.svg')" alt=""
          class="xl:absolute xl:right-[189px] xl:bottom-[299px] hidden z-10">
      </section>
      <!-- banner section end -->

      <!-- feature and brand area start -->
      <section class="-mt-[75px] relative z-50">
        <div class="container px-3 md:px-5 xl:px-0">
          <div
            class="bg-white shadow-[0px_24px_100px_rgba(22,25,50,0.07)] rounded-xl xl:py-[50px] xl:px-[70px] p-8 mb-[26px]">
            <div class="grid grid-cols-1 xl:grid-cols-4 sm:grid-cols-2 gap-6">
              <div class="feature-card flex gap-4 items-center w-full max-w-[280px]">
                <div>
                  <svg width="46" height="46" viewBox="0 0 46 46" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_248_4580)">
                      <path
                        d="M44.1788 10.1498L23.293 0.0669785C23.1078 -0.0223262 22.8922 -0.0223262 22.7071 0.0669785L1.82125 10.1498C1.58837 10.2622 1.4404 10.498 1.4404 10.7566V35.2434C1.4404 35.502 1.58837 35.7378 1.82125 35.8502L22.707 45.933C22.7996 45.9777 22.8999 46 23 46C23.1002 46 23.2004 45.9777 23.293 45.933L44.1788 35.8502C44.4117 35.7378 44.5597 35.502 44.5597 35.2434V10.7567C44.5597 10.4979 44.4116 10.2623 44.1788 10.1498ZM23 1.42209L42.3359 10.7566L36.7308 13.4625C36.6954 13.4355 36.6579 13.4105 36.6167 13.3906L17.4122 4.11965L23 1.42209ZM15.8904 4.88153L35.1982 14.2025L31.2437 16.1115L11.9439 6.79439L15.8904 4.88153ZM35.6499 15.4808V22.5376L31.9562 24.3208V17.264L35.6499 15.4808ZM43.212 34.8206L23.6739 44.2526V21.2623L28.3343 19.0124C28.6694 18.8506 28.8099 18.4478 28.6481 18.1126C28.4863 17.7776 28.0836 17.6369 27.7484 17.7988L23 20.0912L21.1316 19.1891C20.7964 19.0272 20.3937 19.1679 20.2318 19.503C20.07 19.8381 20.2106 20.2409 20.5457 20.4028L22.3262 21.2623V44.2526L2.78806 34.8204V11.8301L17.6662 19.0127C17.7606 19.0583 17.8604 19.0799 17.9586 19.0799C18.2091 19.0799 18.4497 18.9396 18.5659 18.6989C18.7277 18.3637 18.5872 17.9609 18.2521 17.7991L3.66412 10.7566L10.3579 7.52509L30.5992 17.2968C30.6022 17.3009 30.6055 17.3046 30.6085 17.3086V25.3945C30.6085 25.6264 30.7278 25.8419 30.9242 25.9652C31.0332 26.0337 31.1577 26.0683 31.2825 26.0683C31.3824 26.0683 31.4825 26.0461 31.5753 26.0013L36.6167 23.5675C36.8496 23.4551 36.9976 23.2194 36.9976 22.9607V14.8303L43.212 11.8302V34.8206Z"
                        fill="#272343" />
                      <path
                        d="M8.34876 32.207L5.28374 30.7274C4.94844 30.5654 4.54576 30.7061 4.38395 31.0412C4.22214 31.3764 4.36266 31.7792 4.69778 31.941L7.7628 33.4206C7.85722 33.4663 7.95704 33.4879 8.05524 33.4879C8.30572 33.4879 8.54633 33.3475 8.66249 33.1068C8.82439 32.7716 8.68388 32.3689 8.34876 32.207Z"
                        fill="#272343" />
                      <path
                        d="M11.1696 30.371L5.28798 27.5315C4.95278 27.3697 4.55001 27.5102 4.3882 27.8454C4.22648 28.1806 4.367 28.5834 4.70211 28.7452L10.5837 31.5847C10.6782 31.6302 10.778 31.6519 10.8762 31.6519C11.1267 31.6519 11.3673 31.5115 11.4834 31.2708C11.6452 30.9355 11.5047 30.5327 11.1696 30.371Z"
                        fill="#272343" />
                    </g>
                    <defs>
                      <clipPath id="clip0_248_4580">
                        <rect width="46" height="46" fill="white" />
                      </clipPath>
                    </defs>
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg leading-[110%] text-gray-black mb-1.5 font-medium">Discount</h3>
                  <p class="text-[#9A9CAA] text-[15px] leading-[110%]">Every week new sales</p>
                </div>
              </div>
              <div class="feature-card flex gap-4 items-center w-full max-w-[280px]">
                <div>
                  <svg width="64" height="39" viewBox="0 0 64 39" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path
                      d="M13.9635 30.5869C12.894 30.5869 12.024 31.4569 12.024 32.5264C12.024 33.5959 12.894 34.4659 13.9635 34.4659C15.033 34.4659 15.903 33.5959 15.903 32.5264C15.903 31.4569 15.033 30.5869 13.9635 30.5869Z"
                      fill="#272343" />
                    <path
                      d="M54.0446 30.5869C52.9751 30.5869 52.1051 31.4569 52.1051 32.5264C52.1051 33.5959 52.9751 34.4659 54.0446 34.4659C55.1141 34.4659 55.9841 33.5959 55.9841 32.5264C55.9841 31.4569 55.1141 30.5869 54.0446 30.5869Z"
                      fill="#272343" />
                    <path
                      d="M61.9886 18.1537L54.7706 15.7477L51.397 6.4705C50.9759 5.31237 49.865 4.53425 48.6326 4.53425H39.9516V2.46562C39.9516 1.39612 39.0816 0.526123 38.0121 0.526123H1.9395C0.87 0.526123 0 1.39625 0 2.46575V29.5202C0 30.5897 0.87 31.4597 1.9395 31.4597H8.11375C8.05075 31.806 8.01612 32.1621 8.01612 32.5262C8.01612 35.8057 10.6842 38.4739 13.9637 38.4739C17.2432 38.4739 19.9114 35.8057 19.9114 32.5262C19.9114 32.162 19.8767 31.806 19.8137 31.4597H48.1946C48.1316 31.806 48.097 32.1621 48.097 32.5262C48.097 35.8057 50.7651 38.4739 54.0446 38.4739C57.3241 38.4739 59.9922 35.8057 59.9922 32.5262C59.9922 32.063 59.9372 31.6125 59.8366 31.1795L61.8205 30.1876C63.1647 29.5152 64 28.1636 64 26.6602V20.9444C64 19.6764 63.1917 18.5549 61.9886 18.1537ZM1.875 2.46575C1.875 2.43012 1.90387 2.40112 1.9395 2.40112H38.0121C38.0477 2.40112 38.0766 2.43 38.0766 2.46562V22.5705H1.875V2.46575ZM13.9636 36.5989C11.718 36.5989 9.891 34.7719 9.891 32.5262C9.891 30.2806 11.718 28.4536 13.9636 28.4536C16.2092 28.4536 18.0362 30.2806 18.0362 32.5262C18.0364 34.7719 16.2094 36.5989 13.9636 36.5989ZM38.0766 29.5846H19.1297C18.1044 27.791 16.1735 26.5786 13.9636 26.5786C11.7537 26.5786 9.823 27.791 8.79762 29.5846H1.9395C1.90387 29.5846 1.875 29.5557 1.875 29.5201V24.4455H38.0766V29.5846ZM50.8372 10.4174L52.706 15.5565H50.693L48.8242 10.4174H50.8372ZM39.9516 6.40925H48.6326C49.0795 6.40925 49.4823 6.69137 49.635 7.11125L50.1554 8.54225H39.9516V6.40925ZM39.9516 10.4174H46.8291L48.6979 15.5565H39.9516V10.4174ZM54.0444 36.5989C51.7988 36.5989 49.9717 34.7719 49.9717 32.5262C49.9717 30.2806 51.7988 28.4536 54.0444 28.4536C56.29 28.4536 58.117 30.2806 58.117 32.5262C58.117 34.7719 56.29 36.5989 54.0444 36.5989ZM62.125 22.5704H61.0585C60.5407 22.5704 60.121 22.9901 60.121 23.5079C60.121 24.0256 60.5407 24.4454 61.0585 24.4454H62.125V26.6601C62.125 27.4489 61.6869 28.1577 60.9816 28.5105L59.1258 29.4384C58.0808 27.725 56.194 26.5786 54.0444 26.5786C51.8345 26.5786 49.9038 27.791 48.8784 29.5846H39.9516V24.4455H57.0505C57.5682 24.4455 57.988 24.0257 57.988 23.508C57.988 22.9902 57.5682 22.5705 57.0505 22.5705H39.9516V17.4314H53.8923L61.3957 19.9325C61.832 20.0779 62.125 20.4845 62.125 20.9442V22.5704Z"
                      fill="#272343" />
                    <path
                      d="M31.4632 11.6718L24.4491 7.66382C23.9997 7.40695 23.427 7.5632 23.17 8.0127C22.9131 8.46232 23.0692 9.03495 23.5189 9.29182L27.4679 11.5484H8.95374C8.43599 11.5484 8.01624 11.9682 8.01624 12.4859C8.01624 13.0037 8.43599 13.4233 8.95374 13.4233H27.4679L23.5189 15.6799C23.0694 15.9368 22.9131 16.5094 23.17 16.9591C23.343 17.2618 23.6594 17.4316 23.9849 17.4316C24.1426 17.4316 24.3025 17.3917 24.4491 17.3078L31.4632 13.2998C31.7552 13.1329 31.9356 12.8223 31.9356 12.4858C31.9356 12.1493 31.7554 11.8388 31.4632 11.6718Z"
                      fill="#272343" />
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg leading-[110%] text-gray-black mb-1.5 font-medium">Free Delivary</h3>
                  <p class="text-[#9A9CAA] text-[15px] leading-[110%]">100% Free for all orders</p>
                </div>
              </div>
              <div class="feature-card flex gap-4 items-center w-full max-w-[280px]">
                <div>
                  <svg width="50" height="50" viewBox="0 0 50 50" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_248_4611)">
                      <path
                        d="M47.5937 14.2852C47.4201 13.9197 46.9829 13.7643 46.6179 13.9379C46.2525 14.1114 46.097 14.5483 46.2705 14.9138C47.7733 18.077 48.5352 21.4705 48.5352 25.0001C48.5352 31.2866 46.0871 37.1968 41.6419 41.642C37.1968 46.0872 31.2865 48.5353 25 48.5353C21.2718 48.5353 17.7063 47.6892 14.403 46.0205C11.6506 44.6301 9.16396 42.678 7.14482 40.3323L10.0346 41.2956C10.4183 41.4235 10.8331 41.2161 10.961 40.8323C11.089 40.4485 10.8815 40.0338 10.4977 39.9059L5.29755 38.1725C5.05673 38.0923 4.7915 38.1423 4.59667 38.305C4.40185 38.4677 4.30507 38.7196 4.34091 38.9709L5.20761 45.0378C5.25985 45.4031 5.57314 45.6667 5.93183 45.6667C5.9663 45.6667 6.00116 45.6643 6.03632 45.6593C6.43681 45.602 6.71503 45.2311 6.65781 44.8307L6.17421 41.4456C8.29326 43.8655 10.8819 45.8829 13.7427 47.328C17.2526 49.1011 21.0401 50.0001 25 50.0001C31.6777 50.0001 37.9559 47.3996 42.6777 42.6778C47.3995 37.9559 50 31.6778 50 25.0001C50 21.2514 49.1904 17.6464 47.5937 14.2852Z"
                        fill="#272343" />
                      <path
                        d="M45.6592 11.0293L44.7925 4.9624C44.7353 4.56191 44.3634 4.28389 43.9639 4.34092C43.5634 4.39814 43.2852 4.76914 43.3424 5.16953L43.8255 8.55117C39.0691 3.10156 32.2791 0 25 0C18.3223 0 12.0442 2.60049 7.32227 7.32227C2.60049 12.0442 0 18.3223 0 25C0 28.7488 0.809668 32.3539 2.40635 35.7149C2.53174 35.9789 2.79443 36.1333 3.06846 36.1333C3.17373 36.1333 3.28076 36.1105 3.38223 36.0622C3.74756 35.8887 3.90303 35.4518 3.72949 35.0863C2.22676 31.9233 1.46484 28.5298 1.46484 25C1.46484 18.7135 3.91289 12.8033 8.35811 8.35811C12.8033 3.91289 18.7135 1.46484 25 1.46484C31.9195 1.46484 38.3694 4.44277 42.8531 9.66709L39.9655 8.70459C39.5815 8.57646 39.1669 8.78408 39.0391 9.16787C38.9112 9.55166 39.1185 9.96641 39.5022 10.0943L44.7024 11.8277C44.7782 11.8529 44.8563 11.8653 44.934 11.8653C45.1031 11.8653 45.2697 11.8067 45.4034 11.6952C45.5982 11.5325 45.695 11.2806 45.6592 11.0293Z"
                        fill="#272343" />
                      <path
                        d="M22.9646 32.8787H15.597C15.8912 30.3152 17.7128 28.5953 19.6318 26.7833C21.6304 24.8962 23.697 22.9449 23.697 20.0146C23.697 17.6116 21.5423 15.6565 18.8939 15.6565C16.2454 15.6565 14.0908 17.6116 14.0908 20.0146C14.0908 20.4191 14.4187 20.747 14.8232 20.747C15.2277 20.747 15.5556 20.4191 15.5556 20.0146C15.5556 18.4193 17.0531 17.1213 18.8939 17.1213C20.7347 17.1213 22.2322 18.4193 22.2322 20.0146C22.2322 22.3134 20.4805 23.9673 18.6261 25.7183C16.5002 27.7255 14.0908 30.0006 14.0908 33.6111C14.0908 34.0156 14.4187 34.3435 14.8232 34.3435H22.9646C23.3691 34.3435 23.697 34.0156 23.697 33.6111C23.697 33.2066 23.3691 32.8787 22.9646 32.8787Z"
                        fill="#272343" />
                      <path
                        d="M35.1767 28.1816H34.3435V16.3889C34.3435 15.9844 34.0157 15.6565 33.6111 15.6565C33.2065 15.6565 32.8787 15.9844 32.8787 16.3889V28.1817H26.6654L28.8511 16.524C28.9257 16.1264 28.6638 15.7436 28.2662 15.6691C27.8691 15.595 27.4861 15.8564 27.4115 16.254L25.063 28.7792C25.0229 28.9933 25.0801 29.2142 25.2193 29.3819C25.3584 29.5496 25.565 29.6465 25.7828 29.6465H32.8787V33.6111C32.8787 34.0155 33.2065 34.3434 33.6111 34.3434C34.0157 34.3434 34.3435 34.0155 34.3435 33.611V29.6464H35.1767C35.5813 29.6464 35.9091 29.3185 35.9091 28.914C35.9091 28.5095 35.5813 28.1816 35.1767 28.1816Z"
                        fill="#272343" />
                      <path
                        d="M25 3.91406C24.5955 3.91406 24.2676 4.24199 24.2676 4.64648V7.77773C24.2676 8.18223 24.5955 8.51016 25 8.51016C25.4046 8.51016 25.7324 8.18223 25.7324 7.77773V4.64648C25.7324 4.24199 25.4046 3.91406 25 3.91406Z"
                        fill="#272343" />
                      <path
                        d="M25 41.4897C24.5955 41.4897 24.2676 41.8177 24.2676 42.2222V45.3534C24.2676 45.7579 24.5955 46.0858 25 46.0858C25.4046 46.0858 25.7324 45.7579 25.7324 45.3534V42.2222C25.7324 41.8177 25.4046 41.4897 25 41.4897Z"
                        fill="#272343" />
                      <path
                        d="M45.3533 24.2676H42.222C41.8175 24.2676 41.4896 24.5955 41.4896 25C41.4896 25.4045 41.8175 25.7324 42.222 25.7324H45.3533C45.7579 25.7324 46.0857 25.4045 46.0857 25C46.0857 24.5955 45.7579 24.2676 45.3533 24.2676Z"
                        fill="#272343" />
                      <path
                        d="M7.77779 24.2676H4.64655C4.24205 24.2676 3.91412 24.5955 3.91412 25C3.91412 25.4045 4.24205 25.7324 4.64655 25.7324H7.77779C8.18229 25.7324 8.51022 25.4045 8.51022 25C8.51022 24.5955 8.18229 24.2676 7.77779 24.2676Z"
                        fill="#272343" />
                    </g>
                    <defs>
                      <clipPath id="clip0_248_4611">
                        <rect width="50" height="50" fill="white" />
                      </clipPath>
                    </defs>
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg leading-[110%] text-gray-black mb-1.5 font-medium">Great Support 24/7</h3>
                  <p class="text-[#9A9CAA] text-[15px] leading-[110%]">We care your experiences</p>
                </div>
              </div>
              <div class="feature-card flex gap-4 items-center w-full max-w-[280px]">
                <div>
                  <svg width="50" height="50" viewBox="0 0 50 50" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <g clip-path="url(#clip0_248_4640)">
                      <path
                        d="M49.2188 6.95611C49.2017 6.63932 48.9825 6.36949 48.6759 6.28785L25.1704 0.0246826C25.0466 -0.00822752 24.9166 -0.00822752 24.7929 0.0246826L1.32403 6.28795C1.01798 6.36969 0.799031 6.63883 0.781453 6.95514C0.765144 7.24811 0.414461 14.2331 3.16123 23.0639C4.77559 28.2539 7.13222 32.9926 10.1658 37.1484C13.9605 42.3471 18.8277 46.6391 24.632 49.9058C24.7434 49.9685 24.8672 50 24.9912 50C25.1091 50 25.2272 49.9715 25.3347 49.9144C31.1488 46.8262 36.0241 42.643 39.8249 37.481C42.8619 33.3563 45.2212 28.6037 46.8372 23.3552C49.5855 14.4291 49.2351 7.25719 49.2188 6.95611ZM45.4219 22.9736C43.8516 28.0558 41.5654 32.6529 38.6267 36.6376C35.1991 41.2852 30.8648 45.1106 25.7327 48.0236V44.2556C32.3859 40.0553 37.4036 34.1094 40.6473 26.5751C43.3181 20.3717 44.1884 14.4831 44.4482 10.6354C44.4718 10.2858 44.2446 9.96841 43.9059 9.87828L42.4122 9.48033C42.0215 9.37623 41.62 9.60855 41.5159 9.99957C41.4117 10.3904 41.6441 10.7918 42.0351 10.896L42.942 11.1376C42.6415 14.8677 41.7552 20.2971 39.3017 25.9958C36.1947 33.2129 31.4039 38.9148 25.0581 42.9508C24.4211 42.5296 23.7946 42.09 23.191 41.6406C22.8667 41.399 22.4077 41.4661 22.166 41.7906C21.9244 42.115 21.9915 42.574 22.316 42.8156C22.9467 43.2853 23.6019 43.7433 24.2675 44.1828V47.9997C19.1331 44.9282 14.7976 41.0013 11.3689 36.3118C8.43114 32.2938 6.1458 27.7075 4.57627 22.6806C2.31719 15.4447 2.20674 9.34488 2.23018 7.56236L24.2675 1.68112V5.02672L6.10468 9.87398C5.76523 9.96461 5.53789 10.2835 5.56289 10.6339C5.75205 13.281 6.28447 17.3995 7.74726 21.9882C10.1655 29.5743 14.227 35.9031 19.8189 40.7989C19.9579 40.9206 20.1299 40.9803 20.3012 40.9803C20.505 40.9803 20.7078 40.8957 20.8527 40.7303C21.1192 40.4259 21.0884 39.9631 20.7841 39.6967C15.3958 34.9793 11.4792 28.8716 9.14306 21.5434C7.83076 17.4267 7.29033 13.7003 7.07148 11.1325L24.9829 6.35241L38.8691 10.0525C39.26 10.1565 39.6614 9.92427 39.7655 9.53326C39.8696 9.14244 39.6372 8.74097 39.2462 8.63687L25.7326 5.036V1.6906L47.7697 7.56266C47.794 9.37564 47.6883 15.6388 45.4219 22.9736Z"
                        fill="#272343" />
                      <path
                        d="M36.0205 17.1149C35.5866 16.6803 35.0093 16.4412 34.3951 16.4412C33.7807 16.4412 33.2035 16.6803 32.77 17.1145L23.4343 26.4497L18.3377 21.3535C17.904 20.9191 17.3266 20.6798 16.7124 20.6798C16.098 20.6798 15.5209 20.919 15.0875 21.353C14.6533 21.7871 14.4139 22.3642 14.4139 22.9783C14.4139 23.5923 14.6531 24.1694 15.0873 24.6033L21.8089 31.3249C22.2427 31.7593 22.8199 31.9986 23.4342 31.9986C24.0486 31.9986 24.6257 31.7594 25.0593 31.3252L36.0199 20.3647C36.4541 19.9308 36.6934 19.3536 36.6934 18.7395C36.6934 18.1254 36.4542 17.5483 36.0205 17.1149ZM34.9841 19.3286L24.0231 30.2896C23.8661 30.4468 23.657 30.5334 23.4342 30.5334C23.2115 30.5334 23.0024 30.4468 22.8451 30.2893L16.123 23.5671C15.9657 23.4099 15.879 23.2008 15.879 22.9782C15.879 22.7555 15.9657 22.5465 16.1235 22.3886C16.2805 22.2314 16.4897 22.1448 16.7124 22.1448C16.9349 22.1448 17.144 22.2314 17.3015 22.3889L22.9165 28.0034C23.2025 28.2895 23.6664 28.2894 23.9523 28.0034L33.8063 18.1499C33.9633 17.9926 34.1725 17.906 34.3952 17.906C34.6178 17.906 34.8268 17.9926 34.9844 18.1503C35.1417 18.3076 35.2285 18.5167 35.2285 18.7393C35.2285 18.9619 35.1417 19.1711 34.9841 19.3286Z"
                        fill="#272343" />
                    </g>
                    <defs>
                      <clipPath id="clip0_248_4640">
                        <rect width="50" height="50" fill="white" />
                      </clipPath>
                    </defs>
                  </svg>
                </div>
                <div>
                  <h3 class="text-lg leading-[110%] text-gray-black mb-1.5 font-medium">secure Payment</h3>
                  <p class="text-[#9A9CAA] text-[15px] leading-[110%]">100% Secure Payment Method</p>
                </div>
              </div>
            </div>
          </div>
          <div class="swiper brandSwiper overflow-hidden">
            <div class="swiper-wrapper items-center" id="brand-swiper">
              <div class="swiper-slide inline-flex items-center justify-center">
                <a href="#"><img :src="require('@/assets/images/all-img/brand-logo-01.png')" alt=""></a>
              </div>
              <div class="swiper-slide inline-flex items-center justify-center">
                <a href="#"><img :src="require('@/assets/images/all-img/brand-logo-02.png')" alt=""></a>
              </div>
              <div class="swiper-slide inline-flex items-center justify-center">
                <a href="#"><img :src="require('@/assets/images/all-img/brand-logo-03.png')" alt=""></a>
              </div>
              <div class="swiper-slide inline-flex items-center justify-center">
                <a href="#"><img :src="require('@/assets/images/all-img/brand-logo-04.png')" alt=""></a>
              </div>
              <div class="swiper-slide inline-flex items-center justify-center">
                <a href="#"><img :src="require('@/assets/images/all-img/brand-logo-05.png')" alt=""></a>
              </div>
              <div class="swiper-slide inline-flex items-center justify-center">
                <a href="#"><img :src="require('@/assets/images/all-img/brand-logo-06.png')" alt=""></a>
              </div>
              <div class="swiper-slide inline-flex items-center justify-center">
                <a href="#"><img :src="require('@/assets/images/all-img/brand-logo-07.png')" alt=""></a>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- feature and brand area end -->

      <!-- feature products section start -->
      <section class="xl:pb-20 pb-8 md:pb-12">
        <div class="container px-3 md:px-5 xl:px-0">
          <div class="flex flex-wrap justify-between items-center mb-10 px-2 xl:px-0">
            <h2 class="text-gray-black xl:text-[32px] xl:leading-[110%] text-xl md:text-2xl font-semibold font-display">
              Featured Products</h2>
            <div class="flex gap-[18px]">
              <button class="featureSwiper-button-prev">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <rect width="24" height="24" transform="matrix(-1 0 0 1 24 0)" fill="none" />
                  <path d="M8.5 7.5L4 12M4 12L8.5 16.5M4 12H20" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
              <button class="featureSwiper-button-next">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M15.5 7.5L20 12M20 12L15.5 16.5M20 12H4" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
            </div>
          </div>
          <div class="swiper featureSwiper overflow-hidden">
            <div class="swiper-wrapper" id="swiper-slide-featured-products">
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-01.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">
                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <button class="cart-icon selected">
                        <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                          xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </a>
                  <div id="heart">
                    <a href="wishlist.html" class="heart-icon">
                      <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd"
                          d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                          stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                      </svg>

                    </a>
                  </div>

                </div>
              </div>

              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-01.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-03.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">
                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>
                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-04.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-03.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">
                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>
                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-03.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-04.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-03.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">
                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>
                  </a>
                </div>
              </div>



            </div>
          </div>
        </div>
      </section>
      <!-- feature products section end -->
      <!-- top categories product section start -->
      <section class="overflow-hidden relative lg:pb-20 md:pb-6 pb-3">
        <div class="container px-3 md:px-5 xl:px-0">
          <div class="flex justify-between items-center mb-10">
            <h2 class="text-gray-black xl:text-[32px] xl:leading-[110%] text-xl md:text-2xl font-semibold font-display">
              Top categories</h2>
            <div class="flex gap-[18px]">
              <button class="categoriesSwiper-button-prev">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <rect width="24" height="24" transform="matrix(-1 0 0 1 24 0)" fill="none" />
                  <path d="M8.5 7.5L4 12M4 12L8.5 16.5M4 12H20" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
              <button class="categoriesSwiper-button-next">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M15.5 7.5L20 12M20 12L15.5 16.5M20 12H4" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
            </div>
          </div>
          <div class="swiper topCategoriesSwiper mx-3 md:mx-0">

            <div class="swiper-wrapper" id="swiper-wrapper-top-categories">


              <div class="swiper-slide">
                <div class="product-card-02">
                  <div class="product-thumb">
                    <a href="products.html"><img :src="require('@/assets/images/all-img/t-product-03.png')" alt=""></a>
                  </div>

                  <div class="product-info">
                    <h2><a href="#">Wing Chair</a></h2>
                    <p>3,584 Products</p>
                  </div>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card-02">
                  <div class="product-thumb">
                    <a href="products.html"><img :src="require('@/assets/images/all-img/t-product-02.png')" alt=""></a>
                  </div>

                  <div class="product-info">
                    <h2><a href="#">Wing Chair</a></h2>
                    <p>3,584 Products</p>
                  </div>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card-02">
                  <div class="product-thumb">
                    <a href="products.html"><img :src="require('@/assets/images/all-img/t-product-03.png')" alt=""></a>
                  </div>

                  <div class="product-info">
                    <h2><a href="#">Wing Chair</a></h2>
                    <p>3,584 Products</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- top categories product section end -->


      <!-- mixit up section start  -->
      <section class="lg:py-20 sm:py-8 py-6">
        <div class="container px-3 md:px-5 xl:px-0">
          <h2
            class="text-gray-black xl:text-[32px] xl:leading-[110%] text-xl md:text-2xl text-center font-semibold font-display mb-4">
            Our Products</h2>
          <ul id="filters" class="flex flex-wrap justify-center gap-2 mb-10">
            <li><button
                class="filter text-[#9A9CAA] text-base leading-[110%] font-display font-medium cursor-pointer p-2 mixitup-control-active"
                data-filter=".all" data-mixitup-control>All</button></li>
            <li><button
                class="filter text-[#9A9CAA] text-base leading-[110%] font-display font-medium cursor-pointer p-2"
                data-filter=".newest">Newest</button></li>
            <li><button
                class="filter text-[#9A9CAA] text-base leading-[110%] font-display font-medium cursor-pointer p-2"
                data-filter=".trending">Trending</button></li>
            <li><button
                class="filter text-[#9A9CAA] text-base leading-[110%] font-display font-medium cursor-pointer p-2"
                data-filter=".best-sellers">Best Sellers</button></li>
            <li><button
                class="filter text-[#9A9CAA] text-base leading-[110%] font-display font-medium cursor-pointer p-2"
                data-filter=".featured">Featured</button></li>
          </ul>

          <div class="portfoliolist justify-center mx-auto" id="portfoliolist">
            <div class="mix all featured portfolio-card" data-cat="featured">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-01.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>

            <div class="mix all trending" data-cat="trending">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-02.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>

            <div class="mix all featured" data-cat="featured">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-03.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>
            <div class="mix all featured portfolio-card" data-cat="featured">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-01.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>
            <div class="mix all best-sellers" data-cat="best-sellers">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-04.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>

            <div class="mix all trending" data-cat="trending">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-04.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>

            <div class="mix all trending" data-cat="trending">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-03.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>

            <div class="mix all best-sellers" data-cat="best-sellers">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-02.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>

            <div class="mix all newest" data-cat="newest">
              <div class="product-card">
                <a href="product-details.html">
                  <div class="product-thumb">
                    <img :src="require('@/assets/images/all-img/f-product-01.png')" alt="">
                    <span class="badge new">New</span>
                  </div>
                  <div class="product-info">
                    <div>
                      <h2 class="product-name">Library Stool Chair</h2>
                      <h3 class="product-price">$20</h3>
                    </div>
                    <div>
                      <button class="cart-icon">
                        <svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                            stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                          <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                            stroke-linecap="round" stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                            fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                            stroke-linejoin="round" />
                        </svg>
                      </button>
                    </div>
                  </div>
                </a>

              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- mixit up section end  -->

      <!-- Testimonials section start -->
      <section class="overflow-hidden lg:py-20 sm:py-8 py-5 bg-[#F0F2F3]">
        <div class="container px-3 md:px-5 xl:px-0">
          <div class="flex flex-wrap justify-between items-center mb-10">
            <h2
              class="text-gray-black xl:text-[32px] xl:leading-[110%] text-xl md:text-2xl font-semibold font-display capitalize">
              What client says about us</h2>
            <div class="flex gap-[18px]">
              <button class="testimonials-button-prev">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <rect width="24" height="24" transform="matrix(-1 0 0 1 24 0)" fill="none" />
                  <path d="M8.5 7.5L4 12M4 12L8.5 16.5M4 12H20" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
              <button class="testimonials-button-next">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M15.5 7.5L20 12M20 12L15.5 16.5M20 12H4" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
            </div>
          </div>
          <div class="swiper testimonialSwiper overflow-hidden">
            <div class="swiper-wrapper" id="testimonials-container">
              <div class="swiper-slide"> <!-- testimonials item start -->
                <div
                  class="testimonial-card bg-white lg:p-10 sm:p-6 p-4 rounded-xl shadow-[0px_8px_40px_rgba(39,35,67,0.08)]">
                  <div class="shadow-[inset_2px_0px_0px_#029FAE] pl-6">
                    <p
                      class="text-[#636270] font-display font-normal lg:text-[20px] lg:leading-[150%] sm:text-base text-sm capitalize">
                      “Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sit amet mi nec massa tincidunt
                      blandit et eu sem. Maecenas laoreet ultrices diam dignissim posuere. Aenean ultrices dui at ipsum
                      sagittis, pharetra lacinia dui faucibus. In ac bibendum ex. Aenean dolor massa, euismod sit amet
                      suscipit et“</p>
                  </div>
                  <div class="flex justify-between items-end">
                    <div class="flex items-center flex-wrap gap-3">
                      <div class="lg:w-[60px] lg:h-[60px] sm:w-12 sm:h-12 w-8 h-8">
                        <img :src="require('@/assets/images/all-img/testimonials.png')" alt=""
                          class="w-full h-full rounded-full">
                      </div>
                      <div>
                        <h4
                          class="xl:text-[20px] xl:leading-[140%] text-sm md:text-base text-gray-black capitalize font-medium font-display">
                          Kristin Watson</h4>
                        <p class="text-[#9A9CAA] lg:text-[16px] lg:leading-[140%] text-sm font-normal font-display">
                          Fashion Designer</p>
                      </div>
                    </div>

                    <span>
                      <svg width="97" height="76" viewBox="0 0 97 76" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                          d="M18.8 37.2824C8.15748 37.2824 0.958313 29.8659 0.958313 18.877C0.958313 8.98829 9.21698 0.75 20.4029 0.75C32.655 0.75 41.7083 10.6387 41.7083 25.7433C41.7083 60.0752 16.6742 73.808 0.958313 75.4583V60.3537C11.6144 58.4316 23.5949 47.7212 24.1315 35.9037C23.5949 36.1753 21.4691 37.2824 18.8 37.2824Z"
                          fill="#F0F2F3" />
                        <path
                          d="M73.1334 37.2824C62.4841 37.2824 55.2917 29.8659 55.2917 18.877C55.2917 8.98829 63.5504 0.75 74.7362 0.75C86.9884 0.75 96.0417 10.6387 96.0417 25.7433C96.0417 60.0752 71.0076 73.808 55.2917 75.4583V60.3537C65.9478 58.4316 77.9283 47.7212 78.4649 35.9037C77.9283 36.1753 75.8025 37.2824 73.1334 37.2824Z"
                          fill="#F0F2F3" />
                      </svg>
                    </span>
                  </div>
                </div>
                <!-- testimonials item end -->
              </div>
              <div class="swiper-slide">
                <!-- testimonials item start -->
                <div
                  class="testimonial-card bg-white lg:p-10 sm:p-6 p-4 rounded-xl shadow-[0px_8px_40px_rgba(39,35,67,0.08)]">
                  <div class="shadow-[inset_2px_0px_0px_#029FAE] pl-6">
                    <p
                      class="text-[#636270] font-display font-normal lg:text-[20px] lg:leading-[150%] sm:text-base text-sm capitalize">
                      “Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sit amet mi nec massa tincidunt
                      blandit et eu sem. Maecenas laoreet ultrices diam dignissim posuere. Aenean ultrices dui at ipsum
                      sagittis, pharetra lacinia dui faucibus. In ac bibendum ex. Aenean dolor massa, euismod sit amet
                      suscipit et“</p>
                  </div>
                  <div class="flex justify-between items-end">
                    <div class="flex items-center flex-wrap gap-3">
                      <div class="lg:w-[60px] lg:h-[60px] sm:w-12 sm:h-12 w-8 h-8">
                        <img :src="require('@/assets/images/all-img/testimonials.png')" alt=""
                          class="w-full h-full rounded-full">
                      </div>
                      <div>
                        <h4
                          class="xl:text-[20px] xl:leading-[140%] text-sm md:text-base text-gray-black capitalize font-medium font-display">
                          Esther Howard</h4>
                        <p class="text-[#9A9CAA] lg:text-[16px] lg:leading-[140%] text-sm font-display">Fashion Designer
                        </p>
                      </div>
                    </div>

                    <span>
                      <svg width="97" height="76" viewBox="0 0 97 76" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                          d="M18.8 37.2824C8.15748 37.2824 0.958313 29.8659 0.958313 18.877C0.958313 8.98829 9.21698 0.75 20.4029 0.75C32.655 0.75 41.7083 10.6387 41.7083 25.7433C41.7083 60.0752 16.6742 73.808 0.958313 75.4583V60.3537C11.6144 58.4316 23.5949 47.7212 24.1315 35.9037C23.5949 36.1753 21.4691 37.2824 18.8 37.2824Z"
                          fill="#F0F2F3" />
                        <path
                          d="M73.1334 37.2824C62.4841 37.2824 55.2917 29.8659 55.2917 18.877C55.2917 8.98829 63.5504 0.75 74.7362 0.75C86.9884 0.75 96.0417 10.6387 96.0417 25.7433C96.0417 60.0752 71.0076 73.808 55.2917 75.4583V60.3537C65.9478 58.4316 77.9283 47.7212 78.4649 35.9037C77.9283 36.1753 75.8025 37.2824 73.1334 37.2824Z"
                          fill="#F0F2F3" />
                      </svg>
                    </span>
                  </div>
                </div>
                <!-- testimonials item end -->
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- Testimonials section end -->

      <!-- recent products section start -->
      <section class="lg:py-20 py-6 sm:py-12">
        <div class="container px-3 md:px-5 xl:px-0">
          <div class="flex justify-between items-center mb-10">
            <h2 class="text-gray-black xl:text-[32px] xl:leading-[110%] text-xl md:text-2xl font-semibold font-display">
              Recently Added</h2>
            <div class="flex gap-[18px]">
              <button class="recentSwiper-button-prev">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <rect width="24" height="24" transform="matrix(-1 0 0 1 24 0)" fill="none" />
                  <path d="M8.5 7.5L4 12M4 12L8.5 16.5M4 12H20" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
              <button class="recentSwiper-button-next">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M15.5 7.5L20 12M20 12L15.5 16.5M20 12H4" stroke="currentColor" stroke-width="1.5"
                    stroke-linecap="round" stroke-linejoin="round" />
                </svg>
              </button>
            </div>
          </div>
          <div class="swiper recentSwiper overflow-hidden">
            <div class="swiper-wrapper" id="swiper-slide-featured-products">

              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-03.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-04.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-01.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
              <div class="swiper-slide">
                <div class="product-card">
                  <a href="product-details.html">
                    <div class="product-thumb">
                      <img :src="require('@/assets/images/all-img/f-product-02.png')" alt="">
                      <span class="badge new">New</span>
                    </div>
                    <div class="product-info">

                      <div class="product-name-price-container">
                        <h2 class="product-name">Library Stool Chair</h2>
                        <h3 class="product-price">$20</h3>
                      </div>
                      <div>
                        <button class="cart-icon">
                          <svg width="30" height="30" id="cart-img" viewBox="0 0 22 22" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <path
                              d="M2.52081 2.97913L4.42748 3.30913L5.31023 13.826C5.34414 14.2399 5.53284 14.6257 5.83867 14.9066C6.14451 15.1875 6.545 15.3427 6.96023 15.3413H16.9611C17.3586 15.3417 17.743 15.1986 18.0435 14.9382C18.344 14.6778 18.5403 14.3177 18.5964 13.9241L19.4672 7.91263C19.4904 7.75275 19.4819 7.58987 19.4421 7.43329C19.4023 7.27671 19.3321 7.12951 19.2354 7.00011C19.1387 6.8707 19.0174 6.76163 18.8785 6.67913C18.7396 6.59663 18.5858 6.54231 18.4259 6.51929C18.3672 6.51288 4.73365 6.50829 4.73365 6.50829"
                              stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            <path d="M12.9479 9.89539H15.4898" stroke="currentColor" stroke-width="1.5"
                              stroke-linecap="round" stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M6.5578 18.5194C6.62502 18.5165 6.69213 18.5272 6.75509 18.551C6.81805 18.5747 6.87556 18.611 6.92414 18.6575C6.97273 18.704 7.01139 18.7599 7.03781 18.8218C7.06422 18.8837 7.07784 18.9503 7.07784 19.0176C7.07784 19.0849 7.06422 19.1515 7.03781 19.2133C7.01139 19.2752 6.97273 19.3311 6.92414 19.3777C6.87556 19.4242 6.81805 19.4605 6.75509 19.4842C6.69213 19.5079 6.62502 19.5187 6.5578 19.5158C6.42936 19.5103 6.30801 19.4554 6.21908 19.3626C6.13015 19.2697 6.08051 19.1461 6.08051 19.0176C6.08051 18.889 6.13015 18.7654 6.21908 18.6726C6.30801 18.5798 6.42936 18.5249 6.5578 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                            <path fill-rule="evenodd" clip-rule="evenodd"
                              d="M16.8988 18.5194C17.0312 18.5194 17.1583 18.572 17.252 18.6657C17.3457 18.7594 17.3983 18.8865 17.3983 19.019C17.3983 19.1515 17.3457 19.2786 17.252 19.3723C17.1583 19.4659 17.0312 19.5186 16.8988 19.5186C16.7663 19.5186 16.6392 19.4659 16.5455 19.3723C16.4518 19.2786 16.3992 19.1515 16.3992 19.019C16.3992 18.8865 16.4518 18.7594 16.5455 18.6657C16.6392 18.572 16.7663 18.5194 16.8988 18.5194Z"
                              fill="#272343" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"
                              stroke-linejoin="round" />
                          </svg>
                        </button>
                      </div>
                    </div>
                  </a>
                  <a href="wishlist.html" class="heart-icon">
                    <svg width="30" height="30" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd"
                        d="M2.63268 10.6315C1.64909 7.56068 2.79768 4.05077 6.02251 3.01218C6.85874 2.74461 7.74682 2.68088 8.61268 2.8263C9.47855 2.97173 10.2971 3.3221 11 3.84818C12.3338 2.81693 14.2743 2.4686 15.9683 3.01218C19.1923 4.05077 20.3491 7.56068 19.3664 10.6315C17.8356 15.499 11 19.2482 11 19.2482C11 19.2482 4.21484 15.5558 2.63268 10.6315V10.6315Z"
                        stroke="#272343" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>

                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <!-- recent products section end -->

      <!-- footer area start -->
      <footer>
        <div class="footer-top xl:pt-20 xl:pb-[60px] py-6 sm:py-8 md:py-12 shadow-[inset_0px_1px_0px_#E1E3E6]">
          <div class="container px-3 md:px-5 xl:px-0">
            <div class=" flex flex-wrap gap-y-6 justify-between">
              <div class="footer-widget max-w-[350px]" id="footer-widget-1">
                <div class="lg:mb-6 mb-4">
                  <a href="#">
                    <img :src="require('@/assets/images/all-img/logo.png')" alt="">
                  </a>
                </div>
                <p class="lg:mb-6 mb-4 text-gray-black text-base">Vivamus tristique odio sit amet velit semper, eu
                  posuere turpis interdum. Cras egestas purus </p>
                <ul class="flex gap-1">
                  <li>
                    <a href="#"
                      class="text-[#636270] p-[11px] rounded-full border border-transparent hover:text-[#007580] hover:border-[#007580] transition-all duration-500">
                      <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <g clip-path="url(#clip0_1101_2875)">
                          <path
                            d="M16 8C16 3.58167 12.4183 0 8 0C3.58167 0 0 3.58167 0 8C0 11.993 2.92533 15.3027 6.75 15.9027V10.3127H4.71867V8H6.75V6.23733C6.75 4.23267 7.94433 3.125 9.77167 3.125C10.6467 3.125 11.5623 3.28133 11.5623 3.28133V5.25H10.5537C9.56 5.25 9.25 5.86667 9.25 6.5V8H11.4687L11.114 10.3127H9.25V15.9027C13.0747 15.3027 16 11.9927 16 8Z"
                            fill="currentColor" />
                        </g>
                        <defs>
                          <clipPath id="clip0_1101_2875">
                            <rect width="16" height="16" fill="white" />
                          </clipPath>
                        </defs>
                      </svg>
                    </a>
                  </li>
                  <li>
                    <a href="#"
                      class="text-[#636270] p-[11px] rounded-full border border-transparent hover:text-[#007580] hover:border-[#007580] transition-all duration-500">
                      <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <g clip-path="url(#clip0_1101_2879)">
                          <path
                            d="M5.03333 14.5001C11.07 14.5001 14.3723 9.49813 14.3723 5.16146C14.3723 5.0208 14.369 4.87713 14.3627 4.73646C15.0052 4.27179 15.5596 3.69621 16 3.0368C15.4017 3.3028 14.7667 3.4768 14.116 3.55213C14.8008 3.14166 15.3136 2.49681 15.5593 1.73713C14.915 2.11902 14.2104 2.38843 13.4757 2.5338C12.9807 2.00757 12.3261 1.65911 11.6132 1.54228C10.9002 1.42546 10.1687 1.54679 9.53161 1.88752C8.89456 2.22824 8.38752 2.76937 8.08891 3.42721C7.79031 4.08506 7.71677 4.82296 7.87967 5.5268C6.575 5.46133 5.29865 5.12242 4.13336 4.53206C2.96806 3.94169 1.93984 3.11303 1.11533 2.0998C0.696305 2.82229 0.568091 3.67723 0.756747 4.49086C0.945403 5.30449 1.43677 6.01576 2.131 6.48013C1.60977 6.46361 1.09995 6.3233 0.643667 6.0708V6.11146C0.643231 6.86962 0.905349 7.60455 1.38547 8.19131C1.86559 8.77808 2.53409 9.18048 3.27733 9.33013C2.79463 9.46221 2.28801 9.48149 1.79667 9.38646C2.00644 10.0385 2.41454 10.6087 2.964 11.0176C3.51346 11.4266 4.17688 11.6537 4.86167 11.6675C4.18054 12.2026 3.40049 12.5981 2.56623 12.8313C1.73197 13.0644 0.859899 13.1306 0 13.0261C1.50191 13.9895 3.24899 14.5012 5.03333 14.5001Z"
                            fill="currentColor" />
                        </g>
                        <defs>
                          <clipPath id="clip0_1101_2879">
                            <rect width="16" height="16" fill="white" />
                          </clipPath>
                        </defs>
                      </svg>
                    </a>
                  </li>
                  <li>
                    <a href="#"
                      class="text-[#636270] p-[11px] rounded-full border border-transparent hover:text-[#007580] hover:border-[#007580] transition-all duration-500">
                      <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                          d="M10.6667 4.66667C10.6667 4.48986 10.7369 4.32029 10.8619 4.19526C10.9869 4.07024 11.1565 4 11.3333 4C11.5101 4 11.6797 4.07024 11.8047 4.19526C11.9298 4.32029 12 4.48986 12 4.66667C12 4.84348 11.9298 5.01305 11.8047 5.13807C11.6797 5.2631 11.5101 5.33333 11.3333 5.33333C11.1565 5.33333 10.9869 5.2631 10.8619 5.13807C10.7369 5.01305 10.6667 4.84348 10.6667 4.66667Z"
                          fill="currentColor" />
                        <path fill-rule="evenodd" clip-rule="evenodd"
                          d="M7.99998 4.83301C7.16013 4.83301 6.35467 5.16664 5.76081 5.7605C5.16694 6.35437 4.83331 7.15982 4.83331 7.99967C4.83331 8.83953 5.16694 9.64498 5.76081 10.2388C6.35467 10.8327 7.16013 11.1663 7.99998 11.1663C8.83983 11.1663 9.64529 10.8327 10.2392 10.2388C10.833 9.64498 11.1666 8.83953 11.1666 7.99967C11.1666 7.15982 10.833 6.35437 10.2392 5.7605C9.64529 5.16664 8.83983 4.83301 7.99998 4.83301ZM5.83331 7.99967C5.83331 7.42504 6.06159 6.87394 6.46792 6.46761C6.87424 6.06128 7.42534 5.83301 7.99998 5.83301C8.57462 5.83301 9.12572 6.06128 9.53204 6.46761C9.93837 6.87394 10.1666 7.42504 10.1666 7.99967C10.1666 8.57431 9.93837 9.12541 9.53204 9.53174C9.12572 9.93807 8.57462 10.1663 7.99998 10.1663C7.42534 10.1663 6.87424 9.93807 6.46792 9.53174C6.06159 9.12541 5.83331 8.57431 5.83331 7.99967Z"
                          fill="currentColor" />
                        <path fill-rule="evenodd" clip-rule="evenodd"
                          d="M11.5053 1.88853C9.17557 1.63026 6.82441 1.63026 4.49465 1.88853C3.15332 2.03853 2.06999 3.09519 1.91265 4.44319C1.63625 6.80625 1.63625 9.19347 1.91265 11.5565C2.06999 12.9045 3.15265 13.9612 4.49465 14.1112C6.80532 14.3692 9.19465 14.3692 11.5053 14.1112C12.8467 13.9612 13.93 12.9045 14.0873 11.5565C14.3638 9.19347 14.3638 6.80625 14.0873 4.44319C13.93 3.09519 12.8473 2.03853 11.5053 1.88853ZM4.60532 2.88186C6.86152 2.63177 9.13845 2.63177 11.3947 2.88186C12.2813 2.98186 12.9913 3.68119 13.0947 4.55986C13.362 6.8454 13.362 9.15431 13.0947 11.4399C12.9913 12.3185 12.2813 13.0185 11.3947 13.1172C9.13845 13.3673 6.86152 13.3673 4.60532 13.1172C3.71865 13.0185 3.00865 12.3185 2.90532 11.4399C2.63802 9.15431 2.63802 6.8454 2.90532 4.55986C3.00865 3.68119 3.71865 2.98119 4.60532 2.88253V2.88186Z"
                          fill="currentColor" />
                      </svg>
                    </a>
                  </li>
                  <li>
                    <a href="#"
                      class="text-[#636270] p-[11px] rounded-full border border-transparent hover:text-[#007580] hover:border-[#007580] transition-all duration-500">
                      <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <g clip-path="url(#clip0_1101_2893)">
                          <path
                            d="M8 0C3.58133 0 0 3.58133 0 8C0 11.3907 2.10933 14.2843 5.08433 15.45C5.01567 14.8157 4.95 13.8467 5.11267 13.1563C5.25933 12.5313 6.05 9.18133 6.05 9.18133C6.05 9.18133 5.80933 8.703 5.80933 7.99367C5.80933 6.88133 6.453 6.05 7.256 6.05C7.93733 6.05 8.26867 6.56267 8.26867 7.178C8.26867 7.86566 7.83133 8.89066 7.60633 9.84066C7.41867 10.6373 8.00633 11.2873 8.79067 11.2873C10.2123 11.2873 11.3063 9.78733 11.3063 7.625C11.3063 5.70933 9.93133 4.36867 7.96567 4.36867C5.69067 4.36867 4.353 6.075 4.353 7.84066C4.353 8.528 4.61867 9.26566 4.95 9.66566C5.01567 9.74366 5.025 9.81566 5.00633 9.89366C4.947 10.147 4.80967 10.6903 4.78433 10.8C4.75 10.9467 4.66867 10.978 4.51567 10.9063C3.51567 10.4407 2.89067 8.98133 2.89067 7.80633C2.89067 5.28133 4.725 2.96567 8.175 2.96567C10.95 2.96567 13.1063 4.94367 13.1063 7.58733C13.1063 10.344 11.3687 12.5623 8.95633 12.5623C8.147 12.5623 7.38433 12.1407 7.122 11.6437C7.122 11.6437 6.722 13.172 6.625 13.547C6.44367 14.2403 5.95633 15.1127 5.63133 15.6437C6.3986 15.8804 7.19706 16.0005 8 16C12.4187 16 16 12.4187 16 8C16 3.58133 12.4187 0 8 0Z"
                            fill="currentColor" />
                        </g>
                        <defs>
                          <clipPath id="clip0_1101_2893">
                            <rect width="16" height="16" fill="white" />
                          </clipPath>
                        </defs>
                      </svg>
                    </a>
                  </li>
                  <li>
                    <a href="#"
                      class="text-[#636270] p-[11px] rounded-full border border-transparent hover:text-[#007580] hover:border-[#007580] transition-all duration-500">
                      <svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                          d="M15.8407 4.80007C15.8407 4.80007 15.6843 3.69674 15.203 3.21274C14.5937 2.57507 13.9123 2.57207 13.6 2.5344C11.3627 2.37207 8.00333 2.37207 8.00333 2.37207H7.99667C7.99667 2.37207 4.63767 2.37207 2.4 2.5344C2.08733 2.57207 1.40633 2.57507 0.796667 3.21274C0.316 3.69674 0.162667 4.80007 0.162667 4.80007C0.162667 4.80007 0 6.09674 0 7.39074V8.60307C0 9.89707 0.159333 11.1937 0.159333 11.1937C0.159333 11.1937 0.315667 12.2971 0.793667 12.7814C1.403 13.4187 2.203 13.3971 2.55933 13.4657C3.84067 13.5877 8 13.6251 8 13.6251C8 13.6251 11.3623 13.6187 13.6 13.4594C13.9127 13.4221 14.5937 13.4187 15.2033 12.7814C15.6843 12.2971 15.8407 11.1937 15.8407 11.1937C15.8407 11.1937 16 9.9004 16 8.6034V7.39107C16 6.0974 15.8407 4.8004 15.8407 4.8004V4.80007ZM6.34667 10.0751V5.5784L10.6683 7.8344L6.34667 10.0751Z"
                          fill="currentColor" />
                      </svg>
                    </a>
                  </li>
                </ul>
              </div>

              <div class="footer-widget" id="footer-widget-2">
                <h2 class="widget-title text-[#9A9CAA] text-sm leading-[110%] font-display font-medium uppercase mb-5">
                  Category</h2>
                <ul class="flex flex-col gap-1 footer-lists">
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1 ease-in-out">Sofa</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">Armchair</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">Wing
                      Chair</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">Desk
                      Chair</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">wooden
                      Chair</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">Park
                      Bench</a>
                  </li>
                </ul>
              </div>

              <div class="footer-widget" id="footer-widget-3">
                <h2 class="widget-title text-[#9A9CAA] text-sm leading-[110%] font-display font-medium uppercase mb-5">
                  Support</h2>
                <ul class="flex flex-col gap-1 footer-lists">
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">Help
                      & Support</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">Tearms
                      & Conditions</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500  inline-block pb-1">Privacy
                      Policy</a>
                  </li>
                  <li>
                    <a href="#"
                      class="footer-link text-gray-black text-base leading-[110%] hover:text-[#007580] transition-all duration-500 inline-block pb-1">Help</a>
                  </li>
                </ul>
              </div>

              <!-- footer newsletter -->
              <div class="footer-widget w-[424px]" id="footer-widget-4">
                <h2 class="widget-title text-[#9A9CAA] text-sm leading-[110%] font-display font-medium uppercase mb-5">
                  Newsletter</h2>
                <form action="" class="flex flex-wrap xl:flex-nowrap gap-1">
                  <input type="text" name="" id=""
                    class="bg-[#FFFFFF] block max-w-[285px] w-full px-5 py-[15px] rounded-lg focus:outline-none focus:ring-2 focus:ring-accents transition duration-300 ease-in-out border border-[#E1E3E6]"
                    placeholder="Your email">
                  <button type="submit" id="subscribe-button">Subscribe</button>
                </form>
                <p class="py-3 text-gray-black opacity-60">Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                  Nullam tincidunt erat enim.</p>
              </div>
              <!-- footer newsletter end -->
            </div>
          </div>
        </div>
        <div class="footer-bottom shadow-[inset_0px_1px_0px_#E1E3E6] py-6">
          <div class="container px-3 md:px-5 xl:px-0">
            <div class="flex flex-wrap sm:justify-between sm:flex-nowrap justify-center items-center gap-y-6">
              <p class="text-center text-[#9A9CAA]">@ 2021 - Blogy - Designed & Develop by <b
                  class="text-grayscales-900">Zakirsoft</b></p>
              <div class="inline-flex justify-center h-[27px] w-[227px]">
                <img :src="require('@/assets/images/all-img/payments.png')" alt="">
              </div>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </div>
</template>
<script>

export default {
  name: "ComfortyHome",
 data() {
  return {
    SubHeaderDropDownIsOpen:false,
  }
 },
    methods: {
        showDropDown(){
          if(!this.SubHeaderDropDownIsOpen){
            document.getElementById('dropdown-for-sub-header').style.left="20%"
             this.SubHeaderDropDownIsOpen=true
          }
          else{
              document.getElementById('dropdown-for-sub-header').style.left="-20%"
              this.SubHeaderDropDownIsOpen=false
          }
        }
  },
};


</script>
<style>
@media (max-width:1023px) {
  .hamburger-btn {
    display: inline-flex;
    flex-direction: column;
    gap: 6px;
  }

  .breadcrumb {
    padding: 48px 0px;
  }
}

@media(max-width:480px) {
  #brand-swiper{
    display:none !important;
  }
  .breadcrumb {
    background-color: var(--bg-breadcum);
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
    padding: 10px 0px;
  }

  .sign_in {
    width: auto;
  }

  .error_wrapper {
    /* padding-top: 202px; */
    padding: 17px 0px;
  }

  .error_wrapper h1 {
    color: var(--gray-black);
    font-weight: 700;
    font-size: 200px;
    line-height: 100%;
    font-family: 'DM Sans';
    text-align: center;
    text-transform: capitalize;
  }

  .error_wrapper p {
    color: var(--gray-black);
    font-weight: 700;
    font-size: 30px;
    line-height: 100%;
    font-family: 'DM Sans';
    text-align: center;
    text-transform: capitalize;
    padding-top: 12px;
  }

  .error_wrapper span {
    color: var(--dark-gray);
    font-weight: 700;
    font-size: 16px;
    line-height: 100%;
    font-family: 'DM Sans';
    text-align: center;
    text-transform: capitalize;
    display: block;
    padding-top: 20px;
  }
}

@media (max-width:380px) {
  
  .nav-menu {
    width: 100%;
  }
}

@media(min-width:1536px) {
  .breadcrumb {
    margin: 0px 4.6%;
  }
}

@media (max-width: 767px) {
  #brand-swiper{
    width:100%;
    height:auto;
    display:flex;
    flex-wrap: wrap;
    justify-content: center;
    gap:0.15rem;
  }
  #brand-swiper div a img{
   width:70px;
  }
  .swiper-button-next,
  .swiper-button-prev {
    display: none;
  }

  .sign_in {
    width: auto;
  }

  .gallery-container,
  .gallery-main {
    width: 100%;
    height: auto;
  }

  .breadcrumb {
    padding: 48px 0px;
  }
}



@media (min-width: 480px) {
  .portfoliolist {
    grid-template-columns: repeat(2, 1fr);
    gap: 12px;
  }
}

@media (min-width: 767px) {
  .portfoliolist {
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
  }
}

@media (min-width: 1024px) {
  .portfoliolist {
    grid-template-columns: repeat(4, 1fr);
    gap: 24px;
  }
}

@media (min-width:1860px) {
  .banner-slider-button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
  }
}

@media (max-width: 1399px) {
  .gallery-container {
    margin: 0px auto 50px;
  }

  .right-side {
    max-width: 730px;
  }
}

@media (max-width:1023px) {
  .hamburger-btn {
    display: inline-flex;
    flex-direction: column;
    gap: 6px;
  }

  .breadcrumb {
    padding: 48px 0px;
  }
}

@media(max-width:480px) {
  .breadcrumb {
    background-color: var(--bg-breadcum);
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
    padding: 10px 0px;
  }

  .sign_in {
    width: auto;
  }

  .error_wrapper {
    /* padding-top: 202px; */
    padding: 17px 0px;
  }

  .error_wrapper h1 {
    color: var(--gray-black);
    font-weight: 700;
    font-size: 200px;
    line-height: 100%;
    font-family: 'DM Sans';
    text-align: center;
    text-transform: capitalize;
  }

  .error_wrapper p {
    color: var(--gray-black);
    font-weight: 700;
    font-size: 30px;
    line-height: 100%;
    font-family: 'DM Sans';
    text-align: center;
    text-transform: capitalize;
    padding-top: 12px;
  }

  .error_wrapper span {
    color: var(--dark-gray);
    font-weight: 700;
    font-size: 16px;
    line-height: 100%;
    font-family: 'DM Sans';
    text-align: center;
    text-transform: capitalize;
    display: block;
    padding-top: 20px;
  }
}

@media (max-width:380px) {
  .nav-menu {
    width: 100%;
  }
}

@media(min-width:1536px) {
  .breadcrumb {
    margin: 0px 4.6%;
  }
}

@media (max-width: 767px) {

  .swiper-button-next,
  .swiper-button-prev {
    display: none;
  }

  .sign_in {
    width: auto;
  }

  .gallery-container,
  .gallery-main {
    width: 100%;
    height: auto;
  }

  .breadcrumb {
    padding: 48px 0px;
  }
}



@media (min-width: 480px) {
  .portfoliolist {
    grid-template-columns: repeat(2, 1fr);
    gap: 12px;
  }
}

@media (min-width: 767px) {
  .portfoliolist {
    grid-template-columns: repeat(3, 1fr);
    gap: 18px;
  }
}

@media (min-width: 1024px) {
  .portfoliolist {
    grid-template-columns: repeat(4, 1fr);
    gap: 24px;
  }
  
}

@media (min-width:1860px) {
  .banner-slider-button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
  }
}

@media (max-width: 1399px) {
  .gallery-container {
    margin: 0px auto 50px;
  }

  .right-side {
    max-width: 730px;
  }
}

/*
! tailwindcss v3.2.1 | MIT License | https://tailwindcss.com
*/

/*
1. Prevent padding and border from affecting element width. (https://github.com/mozdevs/cssremedy/issues/4)
2. Allow adding a border to an element by just adding a border-width. (https://github.com/tailwindcss/tailwindcss/pull/116)
*/

*,
::before,
::after {
  box-sizing: border-box;
  /* 1 */
  border-width: 0;
  /* 2 */
  border-style: solid;
  /* 2 */
  border-color: currentColor;
  /* 2 */
}

::before,
::after {
  --tw-content: '';
}

/*
1. Use a consistent sensible line-height in all browsers.
2. Prevent adjustments of font size after orientation changes in iOS.
3. Use a more readable tab size.
4. Use the user's configured `sans` font-family by default.
*/

html {
  line-height: 1.5;
  /* 1 */
  -webkit-text-size-adjust: 100%;
  /* 2 */
  -moz-tab-size: 4;
  /* 3 */
  -o-tab-size: 4;
  tab-size: 4;
  /* 3 */
  font-family: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
  /* 4 */
}

/*
1. Remove the margin in all browsers.
2. Inherit line-height from `html` so users can set them as a class directly on the `html` element.
*/

body {
  margin: 0;
  /* 1 */
  line-height: inherit;
  /* 2 */
}

/*
1. Add the correct height in Firefox.
2. Correct the inheritance of border color in Firefox. (https://bugzilla.mozilla.org/show_bug.cgi?id=190655)
3. Ensure horizontal rules are visible by default.
*/

hr {
  height: 0;
  /* 1 */
  color: inherit;
  /* 2 */
  border-top-width: 1px;
  /* 3 */
}

/*
Add the correct text decoration in Chrome, Edge, and Safari.
*/

abbr:where([title]) {
  -webkit-text-decoration: underline dotted;
  text-decoration: underline dotted;
}

/*
Remove the default font size and weight for headings.
*/

h1,
h2,
h3,
h4,
h5,
h6 {
  font-size: inherit;
  font-weight: inherit;
}

/*
Reset links to optimize for opt-in styling instead of opt-out.
*/

a {
  color: inherit;
  text-decoration: inherit;
}

/*
Add the correct font weight in Edge and Safari.
*/

b,
strong {
  font-weight: bolder;
}

/*
1. Use the user's configured `mono` font family by default.
2. Correct the odd `em` font sizing in all browsers.
*/

code,
kbd,
samp,
pre {
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
  /* 1 */
  font-size: 1em;
  /* 2 */
}

/*
Add the correct font size in all browsers.
*/

small {
  font-size: 80%;
}

/*
Prevent `sub` and `sup` elements from affecting the line height in all browsers.
*/

sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}

sub {
  bottom: -0.25em;
}

sup {
  top: -0.5em;
}

/*
1. Remove text indentation from table contents in Chrome and Safari. (https://bugs.chromium.org/p/chromium/issues/detail?id=999088, https://bugs.webkit.org/show_bug.cgi?id=201297)
2. Correct table border color inheritance in all Chrome and Safari. (https://bugs.chromium.org/p/chromium/issues/detail?id=935729, https://bugs.webkit.org/show_bug.cgi?id=195016)
3. Remove gaps between table borders by default.
*/

table {
  text-indent: 0;
  /* 1 */
  border-color: inherit;
  /* 2 */
  border-collapse: collapse;
  /* 3 */
}

/*
1. Change the font styles in all browsers.
2. Remove the margin in Firefox and Safari.
3. Remove default padding in all browsers.
*/

button,
input,
optgroup,
select,
textarea {
  font-family: inherit;
  /* 1 */
  font-size: 100%;
  /* 1 */
  font-weight: inherit;
  /* 1 */
  line-height: inherit;
  /* 1 */
  color: inherit;
  /* 1 */
  margin: 0;
  /* 2 */
  padding: 0;
  /* 3 */
}

/*
Remove the inheritance of text transform in Edge and Firefox.
*/

button,
select {
  text-transform: none;
}

/*
1. Correct the inability to style clickable types in iOS and Safari.
2. Remove default button styles.
*/

button,
[type='button'],
[type='reset'],
[type='submit'] {
  /* -webkit-appearance: button;
/* 1 */
  background-color: transparent;
  /* 2 */
  background-image: none;
  /* 2 */
}

*/
/*
Use the modern Firefox focus style for all focusable elements.
*/

:-moz-focusring {
  outline: auto;
}

/*
Remove the additional `:invalid` styles in Firefox. (https://github.com/mozilla/gecko-dev/blob/2f9eacd9d3d995c937b4251a5557d95d494c9be1/layout/style/res/forms.css#L728-L737)
*/

:-moz-ui-invalid {
  box-shadow: none;
}

/*
Add the correct vertical alignment in Chrome and Firefox.
*/

progress {
  vertical-align: baseline;
}

/*
Correct the cursor style of increment and decrement buttons in Safari.
*/

::-webkit-inner-spin-button,
::-webkit-outer-spin-button {
  height: auto;
}

/*
1. Correct the odd appearance in Chrome and Safari.
2. Correct the outline style in Safari.
*/

[type='search'] {
  /* -webkit-appearance: textfield;
/* 1 */
  outline-offset: -2px;
  /* 2 */
}

*/
/*
Remove the inner padding in Chrome and Safari on macOS.
*/

::-webkit-search-decoration {
  -webkit-appearance: none;
}

/*
1. Correct the inability to style clickable types in iOS and Safari.
2. Change font properties to `inherit` in Safari.
*/

::-webkit-file-upload-button {
  -webkit-appearance: button;
  /* 1 */
  font: inherit;
  /* 2 */
}

/*
Add the correct display in Chrome and Safari.
*/

summary {
  display: list-item;
}

/*
Removes the default spacing and border for appropriate elements.
*/

blockquote,
dl,
dd,
h1,
h2,
h3,
h4,
h5,
h6,
hr,
figure,
p,
pre {
  margin: 0;
}

fieldset {
  margin: 0;
  padding: 0;
}

legend {
  padding: 0;
}

ol,
ul,
menu {
  list-style: none;
  margin: 0;
  padding: 0;
}

/*
Prevent resizing textareas horizontally by default.
*/

textarea {
  resize: vertical;
}

/*
1. Reset the default placeholder opacity in Firefox. (https://github.com/tailwindlabs/tailwindcss/issues/3300)
2. Set the default placeholder color to the user's configured gray 400 color.
*/

input::-moz-placeholder,
textarea::-moz-placeholder {
  opacity: 1;
  /* 1 */
  color: #9ca3af;
  /* 2 */
}

input::placeholder,
textarea::placeholder {
  opacity: 1;
  /* 1 */
  color: #9ca3af;
  /* 2 */
}

/*
Set the default cursor for buttons.
*/

button,
[role="button"] {
  cursor: pointer;
}

/*
Make sure disabled buttons don't get the pointer cursor.
*/

:disabled {
  cursor: default;
}

/*
1. Make replaced elements `display: block` by default. (https://github.com/mozdevs/cssremedy/issues/14)
2. Add `vertical-align: middle` to align replaced elements more sensibly by default. (https://github.com/jensimmons/cssremedy/issues/14#issuecomment-634934210)
 This can trigger a poorly considered lint error in some tools but is included by design.
*/

img,
svg,
video,
canvas,
audio,
iframe,
embed,
object {
  display: block;
  /* 1 */
  /* vertical-align: middle; */
  /* 2 */
}

/*
Constrain images and videos to the parent width and preserve their intrinsic aspect ratio. (https://github.com/mozdevs/cssremedy/issues/14)
*/

img,
video {
  max-width: 90%;
  height: auto;
}

/* Make elements with the HTML hidden attribute stay hidden by default */

[hidden] {
  display: none;
}



.container {
  width: 100%;
  margin-right: auto;
  margin-left: auto;
  padding-right: 0rem;
  padding-left: 0rem;
}

@media (min-width: 600px) {
  .container {
    max-width: 600px;
  }
}

@media (min-width: 728px) {
  .container {
    max-width: 728px;
  }
}

@media (min-width: 920px) {
  .container {
    max-width: 920px;
  }
}

@media (min-width: 980px) {
  .container {
    max-width: 980px;
  }
}

@media (min-width: 1320px) {
  .container {
    max-width: 1320px;
  }
}

.visible {
  visibility: visible;
}

.static {
  position: static;
}

.fixed {
  position: fixed;
}

.absolute {
  position: absolute;
}

.relative {
  position: relative;
}

.right-4 {
  right: 1rem;
}

.top-3 {
  top: 0.75rem;
}

.-top-1 {
  top: -0.25rem;
}

.right-0 {
  right: 0px;
}

.top-0 {
  top: 0px;
}

.top-\[33px\] {
  top: 33px;
}

.right-9 {
  right: 2.25rem;
}

.top-\[68px\] {
  top: 68px;
}

.right-10 {
  right: 2.5rem;
}

.top-\[17px\] {
  top: 17px;
}

.right-5 {
  right: 1.25rem;
}

.top-\[18px\] {
  top: 18px;
}

.isolate {
  isolation: isolate;
}

.z-30 {
  z-index: 30;
}

.z-10 {
  z-index: 10;
}

.z-50 {
  z-index: 50;
}

.m-0 {
  margin: 0px;
}

.m-1 {
  margin: 0.25rem;
}

.mx-3 {
  margin-left: 0.75rem;
  margin-right: 0.75rem;
}

.mx-auto {
  margin-left: auto;
  margin-right: auto;
}

.my-0 {
  margin-top: 0px;
  margin-bottom: 0px;
}

.my-8 {
  margin-top: 2rem;
  margin-bottom: 2rem;
}

.ml-1 {
  margin-left: 0.25rem;
}

.mb-0 {
  margin-bottom: 0px;
}

.mb-4 {
  margin-bottom: 1rem;
}

.mb-2 {
  margin-bottom: 0.5rem;
}

.mb-6 {
  margin-bottom: 1.5rem;
}

.-mt-\[75px\] {
  margin-top: -75px;
}

.mb-\[26px\] {
  margin-bottom: 26px;
}

.mb-1\.5 {
  margin-bottom: 0.375rem;
}

.mb-1 {
  margin-bottom: 0.25rem;
}

.mb-10 {
  margin-bottom: 2.5rem;
}

.mb-5 {
  margin-bottom: 1.25rem;
}

.mt-\[10px\] {
  margin-top: 10px;
}

.mt-6 {
  margin-top: 1.5rem;
}

.ml-2 {
  margin-left: 0.5rem;
}

.mt-5 {
  margin-top: 1.25rem;
}

.mb-\[50px\] {
  margin-bottom: 50px;
}

.mb-3\.5 {
  margin-bottom: 0.875rem;
}

.mb-3 {
  margin-bottom: 0.75rem;
}

.block {
  display: block;
}

.inline-block {
  display: inline-block;
}

.inline {
  display: inline;
}

.flex {
  display: flex;
}

.inline-flex {
  display: inline-flex;
}

.table {
  display: table;
}

.grid {
  display: grid;
}

.contents {
  display: contents;
}

.hidden {
  display: none;
}

.h-\[44px\] {
  height: 44px;
}

.h-8 {
  height: 2rem;
}

.h-full {
  height: 100%;
}

.h-\[27px\] {
  height: 27px;
}

.h-\[50px\] {
  height: 50px;
}

.h-\[150px\] {
  height: 150px;
}

.h-\[70px\] {
  height: 70px;
}

.h-4 {
  height: 1rem;
}

.h-\[1px\] {
  height: 1px;
}

.h-auto {
  height: auto;
}

.h-\[52px\] {
  height: 52px;
}

.h-5 {
  height: 1.25rem;
}

.w-full {
  width: 100%;
}

.w-\[44px\] {
  width: 44px;
}

.w-1\/2 {
  width: 50%;
}

.w-8 {
  width: 2rem;
}

.w-\[424px\] {
  width: 424px;
}

.w-\[227px\] {
  width: 227px;
}

.w-\[150px\] {
  width: 150px;
}

.w-\[160px\] {
  width: 160px;
}

.w-\[200px\] {
  width: 200px;
}

.w-\[140px\] {
  width: 140px;
}

.w-\[120px\] {
  width: 120px;
}

.w-\[100px\] {
  width: 100px;
}

.w-\[305px\] {
  width: 305px;
}

.w-\[145px\] {
  width: 145px;
}

.w-\[175px\] {
  width: 175px;
}

.w-\[295px\] {
  width: 295px;
}

.w-\[340px\] {
  width: 340px;
}

.w-\[104px\] {
  width: 104px;
}

.w-\[70px\] {
  width: 70px;
}

.w-4 {
  width: 1rem;
}

.w-5 {
  width: 1.25rem;
}

.w-\[52px\] {
  width: 52px;
}

.w-\[824px\] {
  width: 824px;
}

.w-\[240px\] {
  width: 240px;
}

.w-\[164px\] {
  width: 164px;
}

.w-\[96px\] {
  width: 96px;
}

.w-\[450px\] {
  width: 450px;
}

.w-\[180px\] {
  width: 180px;
}

.min-w-\[1240px\] {
  min-width: 1240px;
}

.min-w-full {
  min-width: 100%;
}

.min-w-\[872px\] {
  min-width: 872px;
}

.min-w-\[1270px\] {
  min-width: 1270px;
}

.max-w-\[280px\] {
  max-width: 280px;
}

.max-w-\[350px\] {
  max-width: 350px;
}

.max-w-\[285px\] {
  max-width: 285px;
}

.max-w-\[348px\] {
  max-width: 348px;
}

.transform {
  transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
}

.cursor-pointer {
  cursor: pointer;
}

.select-none {
  -webkit-user-select: none;
  -moz-user-select: none;
  user-select: none;
}

.resize {
  resize: both;
}

.grid-cols-1 {
  grid-template-columns: repeat(1, minmax(0, 1fr));
}

.flex-row {
  flex-direction: row;
}

.flex-col {
  flex-direction: column;
}

.flex-wrap {
  flex-wrap: wrap;
}

.items-start {
  align-items: flex-start;
}

.items-end {
  align-items: flex-end;
}

.items-center {
  align-items: center;
}

.justify-center {
  justify-content: center;
}

.justify-between {
  justify-content: space-between;
}

.justify-around {
  justify-content: space-around;
}

.gap-2 {
  gap: 0.5rem;
}

.gap-6 {
  gap: 1.5rem;
}

.gap-3 {
  gap: 0.75rem;
}

.gap-1 {
  gap: 0.25rem;
}

.gap-8 {
  gap: 2rem;
}

.gap-4 {
  gap: 1rem;
}

.gap-\[18px\] {
  gap: 18px;
}

.gap-5 {
  gap: 1.25rem;
}

.gap-\[27px\] {
  gap: 27px;
}

.gap-\[6px\] {
  gap: 6px;
}

.gap-2\.5 {
  gap: 0.625rem;
}

.gap-1\.5 {
  gap: 0.375rem;
}

.gap-\[30px\] {
  gap: 30px;
}

.gap-y-6 {
  row-gap: 1.5rem;
}

.gap-y-4 {
  row-gap: 1rem;
}

.gap-y-2 {
  row-gap: 0.5rem;
}

.gap-x-6 {
  -moz-column-gap: 1.5rem;
  column-gap: 1.5rem;
}

.overflow-hidden {
  overflow: hidden;
}

.overflow-x-auto {
  overflow-x: auto;
}

.rounded-lg {
  border-radius: 0.5rem;
}

.rounded-full {
  border-radius: 9999px;
}

.rounded-md {
  border-radius: 0.375rem;
}

.rounded-none {
  border-radius: 0px;
}

.rounded-xl {
  border-radius: 0.75rem;
}

.rounded {
  border-radius: 0.25rem;
}

.rounded-\[4px\] {
  border-radius: 4px;
}

.rounded-bl-\[20px\] {
  border-bottom-left-radius: 20px;
}

.rounded-br-\[20px\] {
  border-bottom-right-radius: 20px;
}

.border-0 {
  border-width: 0px;
}

.border {
  border-width: 1px;
}

.border-b-2 {
  border-bottom-width: 2px;
}

.border-b {
  border-bottom-width: 1px;
}

.border-none {
  border-style: none;
}

.border-grayscales-700 {
  --tw-border-opacity: 1;
  border-color: rgb(225 227 230 / var(--tw-border-opacity));
}

.border-\[\#029FAE\] {
  --tw-border-opacity: 1;
  border-color: rgb(2 159 174 / var(--tw-border-opacity));
}

.border-transparent {
  border-color: transparent;
}

.border-\[\#E1E3E6\] {
  --tw-border-opacity: 1;
  border-color: rgb(225 227 230 / var(--tw-border-opacity));
}

.border-accents {
  --tw-border-opacity: 1;
  border-color: rgb(2 159 174 / var(--tw-border-opacity));
}

.border-gray-black {
  --tw-border-opacity: 1;
  border-color: rgb(39 35 67 / var(--tw-border-opacity));
}

.border-\[\#D6D9DD\] {
  --tw-border-opacity: 1;
  border-color: rgb(214 217 221 / var(--tw-border-opacity));
}

.bg-secondary {
  --tw-bg-opacity: 1;
  background-color: rgb(39 35 67 / var(--tw-bg-opacity));
}

.bg-grayscales-500 {
  --tw-bg-opacity: 1;
  background-color: rgb(240 242 243 / var(--tw-bg-opacity));
}

.bg-white {
  --tw-bg-opacity: 1;
  background-color: rgb(255 255 255 / var(--tw-bg-opacity));
}

.bg-dark-accents {
  --tw-bg-opacity: 1;
  background-color: rgb(0 117 128 / var(--tw-bg-opacity));
}

.bg-transparent {
  background-color: transparent;
}

.bg-\[\#F7F7F9\] {
  --tw-bg-opacity: 1;
  background-color: rgb(247 247 249 / var(--tw-bg-opacity));
}

.bg-\[\#F0F2F3\] {
  --tw-bg-opacity: 1;
  background-color: rgb(240 242 243 / var(--tw-bg-opacity));
}

.bg-\[\#FFFFFF\] {
  --tw-bg-opacity: 1;
  background-color: rgb(255 255 255 / var(--tw-bg-opacity));
}

.bg-accents {
  --tw-bg-opacity: 1;
  background-color: rgb(2 159 174 / var(--tw-bg-opacity));
}

.bg-off-white {
  --tw-bg-opacity: 1;
  background-color: rgb(240 242 243 / var(--tw-bg-opacity));
}

.bg-\[\#F5813F\] {
  --tw-bg-opacity: 1;
  background-color: rgb(245 129 63 / var(--tw-bg-opacity));
}

.bg-\[\#1E1E1E\] {
  --tw-bg-opacity: 1;
  background-color: rgb(30 30 30 / var(--tw-bg-opacity));
}

.bg-\[\#B26F3F\] {
  --tw-bg-opacity: 1;
  background-color: rgb(178 111 63 / var(--tw-bg-opacity));
}

.bg-\[\#F7AD94\] {
  --tw-bg-opacity: 1;
  background-color: rgb(247 173 148 / var(--tw-bg-opacity));
}

.bg-\[\#029FAE\] {
  --tw-bg-opacity: 1;
  background-color: rgb(2 159 174 / var(--tw-bg-opacity));
}

.bg-\[\#007580\] {
  --tw-bg-opacity: 1;
  background-color: rgb(0 117 128 / var(--tw-bg-opacity));
}

.object-cover {
  -o-object-fit: cover;
  object-fit: cover;
}

.p-\[11px\] {
  padding: 11px;
}

.p-6 {
  padding: 1.5rem;
}

.p-2 {
  padding: 0.5rem;
}

.p-3 {
  padding: 0.75rem;
}

.p-8 {
  padding: 2rem;
}

.p-4 {
  padding: 1rem;
}

.p-5 {
  padding: 1.25rem;
}

.p-0 {
  padding: 0px;
}

.px-3 {
  padding-left: 0.75rem;
  padding-right: 0.75rem;
}

.py-3\.5 {
  padding-top: 0.875rem;
  padding-bottom: 0.875rem;
}

.py-3 {
  padding-top: 0.75rem;
  padding-bottom: 0.75rem;
}

.py-5 {
  padding-top: 1.25rem;
  padding-bottom: 1.25rem;
}

.px-4 {
  padding-left: 1rem;
  padding-right: 1rem;
}

.py-\[3px\] {
  padding-top: 3px;
  padding-bottom: 3px;
}

.px-\[9px\] {
  padding-left: 9px;
  padding-right: 9px;
}

.px-2 {
  padding-left: 0.5rem;
  padding-right: 0.5rem;
}

.py-4 {
  padding-top: 1rem;
  padding-bottom: 1rem;
}

.py-2 {
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
}

.px-6 {
  padding-left: 1.5rem;
  padding-right: 1.5rem;
}

.py-1\.5 {
  padding-top: 0.375rem;
  padding-bottom: 0.375rem;
}

.py-1 {
  padding-top: 0.25rem;
  padding-bottom: 0.25rem;
}

.py-6 {
  padding-top: 1.5rem;
  padding-bottom: 1.5rem;
}

.px-5 {
  padding-left: 1.25rem;
  padding-right: 1.25rem;
}

.py-\[15px\] {
  padding-top: 15px;
  padding-bottom: 15px;
}

.py-\[150px\] {
  padding-top: 150px;
  padding-bottom: 150px;
}

.py-\[1\.5px\] {
  padding-top: 1.5px;
  padding-bottom: 1.5px;
}

.py-10 {
  padding-top: 2.5rem;
  padding-bottom: 2.5rem;
}

.py-\[17px\] {
  padding-top: 17px;
  padding-bottom: 17px;
}

.px-8 {
  padding-left: 2rem;
  padding-right: 2rem;
}

.py-\[30px\] {
  padding-top: 30px;
  padding-bottom: 30px;
}

.py-8 {
  padding-top: 2rem;
  padding-bottom: 2rem;
}

.py-20 {
  padding-top: 5rem;
  padding-bottom: 5rem;
}

.py-\[16px\] {
  padding-top: 16px;
  padding-bottom: 16px;
}

.px-0 {
  padding-left: 0px;
  padding-right: 0px;
}

.px-2\.5 {
  padding-left: 0.625rem;
  padding-right: 0.625rem;
}

.py-\[18px\] {
  padding-top: 18px;
  padding-bottom: 18px;
}

.py-\[19px\] {
  padding-top: 19px;
  padding-bottom: 19px;
}

.pb-4 {
  padding-bottom: 1rem;
}

.pb-8 {
  padding-bottom: 2rem;
}

.pb-3 {
  padding-bottom: 0.75rem;
}

.pl-6 {
  padding-left: 1.5rem;
}

.pb-1 {
  padding-bottom: 0.25rem;
}

.pb-5 {
  padding-bottom: 1.25rem;
}

.pt-\[13\.5px\] {
  padding-top: 13.5px;
}

.pl-5 {
  padding-left: 1.25rem;
}

.pb-\[26px\] {
  padding-bottom: 26px;
}

.pt-10 {
  padding-top: 2.5rem;
}

.pb-20 {
  padding-bottom: 5rem;
}

.pb-6 {
  padding-bottom: 1.5rem;
}

.pb-\[10px\] {
  padding-bottom: 10px;
}

.pt-4 {
  padding-top: 1rem;
}

.pt-6 {
  padding-top: 1.5rem;
}

.pt-5 {
  padding-top: 1.25rem;
}

.pb-2 {
  padding-bottom: 0.5rem;
}

.pt-\[34px\] {
  padding-top: 34px;
}

.pr-5 {
  padding-right: 1.25rem;
}

.pl-\[14px\] {
  padding-left: 14px;
}

.pr-\[14px\] {
  padding-right: 14px;
}

.text-left {
  text-align: left;
}

.text-center {
  text-align: center;
}

.text-right {
  text-align: right;
}

.text-start {
  text-align: start;
}

.font-display {
  font-family: 'Inter', sans-serif;
}

.font-display2 {
  font-family: 'DM Sans', sans-serif;
}

.text-\[13px\] {
  font-size: 13px;
}

.text-\[10px\] {
  font-size: 10px;
}

.text-lg {
  font-size: 1.125rem;
  line-height: 1.75rem;
}

.text-xl {
  font-size: 1.25rem;
  line-height: 1.75rem;
}

.text-sm {
  font-size: 0.875rem;
  line-height: 1.25rem;
}

.text-4xl {
  font-size: 2.25rem;
  line-height: 2.5rem;
}

.text-\[15px\] {
  font-size: 15px;
}

.text-base {
  font-size: 1rem;
  line-height: 1.5rem;
}

.text-\[288px\] {
  font-size: 288px;
}

.text-\[40px\] {
  font-size: 40px;
}

.text-\[18px\] {
  font-size: 18px;
}

.text-\[14px\] {
  font-size: 14px;
}

.text-\[16px\] {
  font-size: 16px;
}

.text-xs {
  font-size: 0.75rem;
  line-height: 1rem;
}

.text-\[20px\] {
  font-size: 20px;
}

.text-\[22px\] {
  font-size: 22px;
}

.text-2xl {
  font-size: 1.5rem;
  line-height: 2rem;
}

.font-semibold {
  font-weight: 600;
}

.font-medium {
  font-weight: 500;
}

.font-bold {
  font-weight: 700;
}

.font-normal {
  font-weight: 400;
}

.uppercase {
  text-transform: uppercase;
}

.capitalize {
  text-transform: capitalize;
}

.leading-\[110\%\] {
  line-height: 110%;
}

.leading-\[130\%\] {
  line-height: 130%;
}

.leading-\[100\%\] {
  line-height: 100%;
}

.leading-\[150\%\] {
  line-height: 150%;
}

.leading-normal {
  line-height: 1.5;
}

.leading-\[120\%\] {
  line-height: 120%;
}

.tracking-\[0\.12em\] {
  letter-spacing: 0.12em;
}

.tracking-wider {
  letter-spacing: 0.05em;
}

.text-white {
  --tw-text-opacity: 1;
  color: rgb(255 255 255 / var(--tw-text-opacity));
}

.text-\[\#272343\] {
  --tw-text-opacity: 1;
  color: rgb(39 35 67 / var(--tw-text-opacity));
}

.text-\[\#636270\] {
  --tw-text-opacity: 1;
  color: rgb(99 98 112 / var(--tw-text-opacity));
}

.text-\[\#9A9CAA\] {
  --tw-text-opacity: 1;
  color: rgb(154 156 170 / var(--tw-text-opacity));
}

.text-grayscales-900 {
  --tw-text-opacity: 1;
  color: rgb(99 98 112 / var(--tw-text-opacity));
}

.text-secondary {
  --tw-text-opacity: 1;
  color: rgb(39 35 67 / var(--tw-text-opacity));
}

.text-black {
  --tw-text-opacity: 1;
  color: rgb(0 0 0 / var(--tw-text-opacity));
}

.text-\[\#F05C52\] {
  --tw-text-opacity: 1;
  color: rgb(240 92 82 / var(--tw-text-opacity));
}

.text-gray-black {
  --tw-text-opacity: 1;
  color: rgb(39 35 67 / var(--tw-text-opacity));
}

.text-dark-gray {
  --tw-text-opacity: 1;
  color: rgb(99 98 112 / var(--tw-text-opacity));
}

.text-\[\#007580\] {
  --tw-text-opacity: 1;
  color: rgb(0 117 128 / var(--tw-text-opacity));
}

.text-\[\#F5813F\] {
  --tw-text-opacity: 1;
  color: rgb(245 129 63 / var(--tw-text-opacity));
}

.text-\[\#01AD5A\] {
  --tw-text-opacity: 1;
  color: rgb(1 173 90 / var(--tw-text-opacity));
}

.text-gray-white {
  --tw-text-opacity: 1;
  color: rgb(255 255 255 / var(--tw-text-opacity));
}

.text-dark-accents {
  --tw-text-opacity: 1;
  color: rgb(0 117 128 / var(--tw-text-opacity));
}

.line-through {
  text-decoration-line: line-through;
}

.opacity-70 {
  opacity: 0.7;
}

.opacity-60 {
  opacity: 0.6;
}

.opacity-30 {
  opacity: 0.3;
}

.shadow-\[0px_1px_0px_\#E1E3E6\] {
  --tw-shadow: 0px 1px 0px #E1E3E6;
  --tw-shadow-colored: 0px 1px 0px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}

.shadow-\[0px_24px_100px_rgba\(22\2c 25\2c 50\2c 0\.07\)\] {
  --tw-shadow: 0px 24px 100px rgba(22, 25, 50, 0.07);
  --tw-shadow-colored: 0px 24px 100px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}

.shadow-\[0px_8px_40px_rgba\(39\2c 35\2c 67\2c 0\.08\)\] {
  --tw-shadow: 0px 8px 40px rgba(39, 35, 67, 0.08);
  --tw-shadow-colored: 0px 8px 40px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}

.shadow-\[inset_2px_0px_0px_\#029FAE\] {
  --tw-shadow: inset 2px 0px 0px #029FAE;
  --tw-shadow-colored: inset 2px 0px 0px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}

.shadow-\[inset_0px_1px_0px_\#E1E3E6\] {
  --tw-shadow: inset 0px 1px 0px #E1E3E6;
  --tw-shadow-colored: inset 0px 1px 0px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}

.shadow {
  --tw-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
  --tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}

.ring-\[\#029FAE\] {
  --tw-ring-opacity: 1;
  --tw-ring-color: rgb(2 159 174 / var(--tw-ring-opacity));
}

.blur {
  --tw-blur: blur(8px);
  filter: var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);
}

.invert {
  --tw-invert: invert(100%);
  filter: var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);
}

.filter {
  filter: var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);
}

.transition-all {
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}

.transition {
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, -webkit-backdrop-filter;
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter;
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter, -webkit-backdrop-filter;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}

.duration-500 {
  transition-duration: 500ms;
}

.duration-300 {
  transition-duration: 300ms;
}

.ease-in-out {
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
}

.hover\:border-\[\#007580\]:hover {
  --tw-border-opacity: 1;
  border-color: rgb(0 117 128 / var(--tw-border-opacity));
}

.hover\:border-\[\#029FAE\]:hover {
  --tw-border-opacity: 1;
  border-color: rgb(2 159 174 / var(--tw-border-opacity));
}

.hover\:bg-\[\#F0F2F3\]:hover {
  --tw-bg-opacity: 1;
  background-color: rgb(240 242 243 / var(--tw-bg-opacity));
}

.hover\:bg-\[\#272343\]:hover {
  --tw-bg-opacity: 1;
  background-color: rgb(39 35 67 / var(--tw-bg-opacity));
}

.hover\:text-\[\#272343\]:hover {
  --tw-text-opacity: 1;
  color: rgb(39 35 67 / var(--tw-text-opacity));
}

.hover\:text-\[\#007580\]:hover {
  --tw-text-opacity: 1;
  color: rgb(0 117 128 / var(--tw-text-opacity));
}

.hover\:text-gray-black:hover {
  --tw-text-opacity: 1;
  color: rgb(39 35 67 / var(--tw-text-opacity));
}

.hover\:text-\[\#029FAE\]:hover {
  --tw-text-opacity: 1;
  color: rgb(2 159 174 / var(--tw-text-opacity));
}

.focus\:outline-none:focus {
  outline: 2px solid transparent;
  outline-offset: 2px;
}

.focus\:ring-2:focus {
  --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);
  --tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);
  box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow), var(--tw-shadow, 0 0 #0000);
}

.focus\:ring:focus {
  --tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);
  --tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);
  box-shadow: var(--tw-ring-offset-shadow), var(--tw-ring-shadow), var(--tw-shadow, 0 0 #0000);
}

.focus\:ring-accents:focus {
  --tw-ring-opacity: 1;
  --tw-ring-color: rgb(2 159 174 / var(--tw-ring-opacity));
}

@media (min-width: 640px) {
  .sm\:flex {
    display: flex;
  }

  .sm\:h-12 {
    height: 3rem;
  }

  .sm\:w-12 {
    width: 3rem;
  }

  .sm\:grid-cols-2 {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .sm\:flex-row {
    flex-direction: row;
  }

  .sm\:flex-nowrap {
    flex-wrap: nowrap;
  }

  .sm\:justify-between {
    justify-content: space-between;
  }

  .sm\:p-6 {
    min-width: 300px;
    padding: 1.5rem;
  }

  .sm\:py-8 {
    padding-top: 2rem;
    padding-bottom: 2rem;
  }

  .sm\:py-12 {
    padding-top: 3rem;
    padding-bottom: 3rem;
  }

  .sm\:text-base {
    font-size: 1rem;
    line-height: 1.5rem;
  }
}

@media (min-width: 768px) {
  .md\:mx-0 {
    margin-left: 0px;
    margin-right: 0px;
  }

  .md\:w-1\/2 {
    width: 50%;
  }

  .md\:grid-cols-3 {
    grid-template-columns: repeat(3, minmax(0, 1fr));
  }

  .md\:flex-row {
    flex-direction: row;
  }

  .md\:flex-wrap {
    flex-wrap: wrap;
  }

  .md\:items-center {
    align-items: center;
  }

  .md\:px-5 {
    padding-left: 1.25rem;
    padding-right: 1.25rem;
  }

  .md\:py-12 {
    padding-top: 3rem;
    padding-bottom: 3rem;
  }

  .md\:px-0 {
    padding-left: 0px;
    padding-right: 0px;
  }

  .md\:py-10 {
    padding-top: 2.5rem;
    padding-bottom: 2.5rem;
  }

  .md\:pb-12 {
    padding-bottom: 3rem;
  }

  .md\:pb-6 {
    padding-bottom: 1.5rem;
  }

  .md\:text-3xl {
    font-size: 1.875rem;
    line-height: 2.25rem;
  }

  .md\:text-2xl {
    font-size: 1.5rem;
    line-height: 2rem;
  }

  .md\:text-base {
    font-size: 1rem;
    line-height: 1.5rem;
  }
}

@media (min-width: 1024px) {
  .lg\:mb-6 {
    margin-bottom: 1.5rem;
  }

  .lg\:block {
    display: block;
  }

  .lg\:flex {
    display: flex;
  }

  .lg\:hidden {
    display: none;
  }

  .lg\:h-\[60px\] {
    height: 60px;
  }

  .lg\:w-\[60px\] {
    width: 60px;
  }

  .lg\:w-2\/3 {
    width: 66.666667%;
  }

  .lg\:w-1\/3 {
    width: 33.333333%;
  }

  .lg\:max-w-\[413px\] {
    max-width: 413px;
  }

  .lg\:flex-row {
    flex-direction: row;
  }

  .lg\:flex-nowrap {
    flex-wrap: nowrap;
  }

  .lg\:justify-between {
    justify-content: space-between;
  }

  .lg\:p-10 {
    padding: 2.5rem;
  }

  .lg\:py-20 {
    padding-top: 5rem;
    padding-bottom: 5rem;
  }

  .lg\:pb-20 {
    padding-bottom: 5rem;
  }

  .lg\:text-\[20px\] {
    font-size: 20px;
  }

  .lg\:text-\[16px\] {
    font-size: 16px;
  }

  .lg\:leading-\[150\%\] {
    line-height: 150%;
  }

  .lg\:leading-\[140\%\] {
    line-height: 140%;
  }
}

@media (min-width: 1280px) {
  .xl\:absolute {
    position: absolute;
  }

  .xl\:right-\[189px\] {
    right: 189px;
  }

  .xl\:bottom-\[299px\] {
    bottom: 299px;
  }

  .xl\:flex {
    display: flex;
  }

  .xl\:w-\[536px\] {
    width: 536px;
  }

  .xl\:w-\[424px\] {
    width: 424px;
  }

  .xl\:w-\[312px\] {
    width: 312px;
  }

  .xl\:w-\[408px\] {
    width: 408px;
  }

  .xl\:w-\[343px\] {
    width: 343px;
  }

  .xl\:w-\[284px\] {
    width: 284px;
  }

  .xl\:max-w-\[732px\] {
    max-width: 732px;
  }

  .xl\:grid-cols-4 {
    grid-template-columns: repeat(4, minmax(0, 1fr));
  }

  .xl\:flex-row {
    flex-direction: row;
  }

  .xl\:flex-nowrap {
    flex-wrap: nowrap;
  }

  .xl\:justify-between {
    justify-content: space-between;
  }

  .xl\:gap-2 {
    gap: 0.5rem;
  }

  .xl\:px-0 {
    padding-left: 0px;
    padding-right: 0px;
  }

  .xl\:py-\[50px\] {
    padding-top: 50px;
    padding-bottom: 50px;
  }

  .xl\:px-\[70px\] {
    padding-left: 70px;
    padding-right: 70px;
  }

  .xl\:px-8 {
    padding-left: 2rem;
    padding-right: 2rem;
  }

  .xl\:py-20 {
    padding-top: 5rem;
    padding-bottom: 5rem;
  }

  .xl\:pt-20 {
    padding-top: 5rem;
  }

  .xl\:pb-28 {
    padding-bottom: 7rem;
  }

  .xl\:pb-20 {
    padding-bottom: 5rem;
  }

  .xl\:pb-\[60px\] {
    padding-bottom: 60px;
  }

  .xl\:pt-10 {
    padding-top: 2.5rem;
  }

  .xl\:text-center {
    text-align: center;
  }

  .xl\:text-\[68px\] {
    font-size: 68px;
  }

  .xl\:text-\[32px\] {
    font-size: 32px;
  }

  .xl\:text-\[20px\] {
    font-size: 20px;
  }

  .xl\:text-2xl {
    font-size: 1.5rem;
    line-height: 2rem;
  }

  .xl\:leading-\[110\%\] {
    line-height: 110%;
  }

  .xl\:leading-\[140\%\] {
    line-height: 140%;
  }
}

@media (min-width: 1536px) {
  .\32xl\:mx-\[90px\] {
    margin-left: 90px;
    margin-right: 90px;
  }

  .\32xl\:max-w-\[424PX\] {
    max-width: 424PX;
  }
}

.p-6 {
  display: none;
}

/* ////////////////////////////////////////////////////////////////////////////////// */
.categoriesSwiper-button-prev {
  padding: 7px;
  background-color: #ff3b00a1;
}

#btn-primary {
  width: 100px !important;
  height: 50px !important;
  display: inline-block;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 17px;
  font-weight: bold;
  color: #f1f1f1;
  background-color: #ff3b00a1;
  border-radius: 5px;
}

#blob {
  background-image: url('../assets/images/svg/blob.svg');
  background-repeat: no-repeat;
  background-size: 107%;
  background-position: top;
  background-position-y: -30px;

}

.testimonials-button-prev,
.featureSwiper-button-prev,
.categoriesSwiper-button-prev,
.recentSwiper-button-prev {
  padding: 7px;
  background-color: #ff3b00a1;
  border-radius: 50%;
  color: white;
}

#home {
  max-width: 100vw;
  margin: 0px;
  padding: 0px;
  overflow-x: hidden
}

#subscribe-button {
  min-width: 150px;
  height: 56px;
  font-size: 17px;
  font-weight: bold;
  color: #f1f1f1;
  background-color: #ff3b00a1;
  border-radius: 5px;
}

.product-card {
  margin-right: 10px;
}

.badge {
  display: none;
}

.cart-icon {
  min-width: 35px;
  padding: 5px;
  border-radius: 5px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.selected {
  background-color: #adecf1;

}

#swiper-slide-2,
#swiper-slide-3 {
  display: none !important;
}

.product-info {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: row;
}

.product-price {
  font-weight: bold;
}

.product-name-price-container {
  width: 70%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin: 5px;
}

.heart-icon {
  position: absolute;
  top: 1vh;
  right: 2vh;
  min-width: 30px;
  background-color: #f5f5f5;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 6px;
  padding: 5px;
}

#swiper-wrapper {
  justify-content: center;
}

#swiper-slide-featured-products {
  flex-wrap: wrap;

  justify-content: center;
}

#swiper-slide-featured-products .swiper-slide {
  margin: 5px;
  padding: 0px;
  min-width: 200px;
}

#swiper-wrapper-top-categories {
  gap: 1rem;
  flex-wrap: wrap;
  justify-content: center;
}

#swiper-wrapper-top-categories .swiper-slide .product-card-02 {
  margin: 5px;
  padding: 0px;
  width: 300px !important;
}

#swiper-wrapper-top-categories .swiper-slide .product-card-02 .product-info a {
  position: absolute;
  font-size: 16px;
  padding: 5px;
  font-weight: bold;
  top: 10px;
  border-radius: 5px;
  color: aliceblue;
  left: 10px;
  background-color: #ff550d6e;
}

#swiper-wrapper-top-categories .swiper-slide .product-card-02 .product-info p {
  font-size: 12px;
  font-weight: bold;
}

.testimonial-card {
  min-width: 450px !important;
  width: 40vw;
  margin: 0px 5px;
}

#portfoliolist {
  width: 100%;
  margin: 0px;
  padding: 0px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

#portfoliolist .product-card {
  margin: 10px;
  min-width: 200px;
  display: flex;
  padding: 0px;
  flex-direction: column;
  align-items: center;
}

.flex-wrap {
  flex-wrap: nowrap !important;
}

#swiper-slide-featured-products {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

#swiper-slide-featured-products .swipe-slide .product-card {
  margin: 10px;
  width: 25vw;
  min-width: 200px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.uppercase {
  font-weight: bold !important;
}

/* ////////////////////////////////////////////////////////////////////////////////////////////// */
/* Responsive */
@media (max-width: 1080px) {

  #footer-widget-1,
  #footer-widget-2,
  #footer-widget-3 {
    display: none;
  }

  #testimonials-container {
    margin: 0px;
    padding: 0px;
    flex-direction: column !important;
    justify-content: center !important;
    gap: 1rem;


  }

  #testimonials-container .swiper-slide {
    display: flex !important;
    justify-content: center !important;
    align-items: center !important;

  }

}

@media (max-width: 768px) {
  #search-input {
    width: 90% !important;
  }

  #responsive-nav {
    display: flex;
    justify-content: center;
    flex-direction: column;
    gap: 1.5rem;
    align-items: center;
  }

  #blob {
    width: 90vw;

  }

  #header-content {
    width: 90vw;

    box-sizing: border-box;

  }

  #swiper-wrapper-top-categories .swiper-slide {
    width: 300px !important;
  }

  .testimonial-card {
    width: 80vw !important;
    min-width: 300px !important;
    width: 40vw;
    margin: 0px 5px;
  }

}

/* ///////////////////////////////////////////////////// */
.select2-container {
  box-sizing: border-box;
  display: inline-block;
  margin: 0;
  position: relative;
  vertical-align: middle
}

.select2-container .select2-selection--single {
  box-sizing: border-box;
  cursor: pointer;
  display: block;
  height: 28px;
  user-select: none;
  -webkit-user-select: none
}

.select2-container .select2-selection--single .select2-selection__rendered {
  display: block;
  padding-left: 8px;
  padding-right: 20px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap
}

.select2-container .select2-selection--single .select2-selection__clear {
  background-color: transparent;
  border: none;
  font-size: 1em
}

.select2-container[dir="rtl"] .select2-selection--single .select2-selection__rendered {
  padding-right: 8px;
  padding-left: 20px
}

.select2-container .select2-selection--multiple {
  box-sizing: border-box;
  cursor: pointer;
  display: block;
  min-height: 32px;
  user-select: none;
  -webkit-user-select: none
}

.select2-container .select2-selection--multiple .select2-selection__rendered {
  display: inline;
  list-style: none;
  padding: 0
}

.select2-container .select2-selection--multiple .select2-selection__clear {
  background-color: transparent;
  border: none;
  font-size: 1em
}

.select2-container .select2-search--inline .select2-search__field {
  box-sizing: border-box;
  border: none;
  font-size: 100%;
  margin-top: 5px;
  margin-left: 5px;
  padding: 0;
  max-width: 100%;
  resize: none;
  height: 18px;
  vertical-align: bottom;
  font-family: sans-serif;
  overflow: hidden;
  word-break: keep-all
}

.select2-container .select2-search--inline .select2-search__field::-webkit-search-cancel-button {
  -webkit-appearance: none
}

.select2-dropdown {
  background-color: white;
  border: 1px solid #aaa;
  border-radius: 4px;
  box-sizing: border-box;
  display: block;
  position: absolute;
  left: -100000px;
  width: 100%;
  z-index: 1051
}

.select2-results {
  display: block
}

.select2-results__options {
  list-style: none;
  margin: 0;
  padding: 0
}

.select2-results__option {
  padding: 6px;
  user-select: none;
  -webkit-user-select: none
}

.select2-results__option--selectable {
  cursor: pointer
}

.select2-container--open .select2-dropdown {
  left: 0
}

.select2-container--open .select2-dropdown--above {
  border-bottom: none;
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0
}

.select2-container--open .select2-dropdown--below {
  border-top: none;
  border-top-left-radius: 0;
  border-top-right-radius: 0
}

.select2-search--dropdown {
  display: block;
  padding: 4px
}

.select2-search--dropdown .select2-search__field {
  padding: 4px;
  width: 100%;
  box-sizing: border-box
}



.select2-search--dropdown.select2-search--hide {
  display: none
}

.select2-close-mask {
  border: 0;
  margin: 0;
  padding: 0;
  display: block;
  position: fixed;
  left: 0;
  top: 0;
  min-height: 100%;
  min-width: 100%;
  height: auto;
  width: auto;
  opacity: 0;
  z-index: 99;
  background-color: #fff;
  filter: alpha(opacity=0)
}

.select2-hidden-accessible {
  border: 0 !important;
  clip: rect(0 0 0 0) !important;
  -webkit-clip-path: inset(50%) !important;
  clip-path: inset(50%) !important;
  height: 1px !important;
  overflow: hidden !important;
  padding: 0 !important;
  position: absolute !important;
  width: 1px !important;
  white-space: nowrap !important
}

.select2-container--default .select2-selection--single {
  background-color: #fff;
  border: 1px solid #aaa;
  border-radius: 4px
}

.select2-container--default .select2-selection--single .select2-selection__rendered {
  color: #444;
  line-height: 28px
}

.select2-container--default .select2-selection--single .select2-selection__clear {
  cursor: pointer;
  float: right;
  font-weight: bold;
  height: 26px;
  margin-right: 20px;
  padding-right: 0px
}

.select2-container--default .select2-selection--single .select2-selection__placeholder {
  color: #999
}

.select2-container--default .select2-selection--single .select2-selection__arrow {
  height: 26px;
  position: absolute;
  top: 1px;
  right: 1px;
  width: 20px
}

.select2-container--default .select2-selection--single .select2-selection__arrow b {
  border-color: #888 transparent transparent transparent;
  border-style: solid;
  border-width: 5px 4px 0 4px;
  height: 0;
  left: 50%;
  margin-left: -4px;
  margin-top: -2px;
  position: absolute;
  top: 50%;
  width: 0
}

.select2-container--default[dir="rtl"] .select2-selection--single .select2-selection__clear {
  float: left
}

.select2-container--default[dir="rtl"] .select2-selection--single .select2-selection__arrow {
  left: 1px;
  right: auto
}

.select2-container--default.select2-container--disabled .select2-selection--single {
  background-color: #eee;
  cursor: default
}

.select2-container--default.select2-container--disabled .select2-selection--single .select2-selection__clear {
  display: none
}

.select2-container--default.select2-container--open .select2-selection--single .select2-selection__arrow b {
  border-color: transparent transparent #888 transparent;
  border-width: 0 4px 5px 4px
}

.select2-container--default .select2-selection--multiple {
  background-color: white;
  border: 1px solid #aaa;
  border-radius: 4px;
  cursor: text;
  padding-bottom: 5px;
  padding-right: 5px;
  position: relative
}

.select2-container--default .select2-selection--multiple.select2-selection--clearable {
  padding-right: 25px
}

.select2-container--default .select2-selection--multiple .select2-selection__clear {
  cursor: pointer;
  font-weight: bold;
  height: 20px;
  margin-right: 10px;
  margin-top: 5px;
  position: absolute;
  right: 0;
  padding: 1px
}

.select2-container--default .select2-selection--multiple .select2-selection__choice {
  background-color: #e4e4e4;
  border: 1px solid #aaa;
  border-radius: 4px;
  box-sizing: border-box;
  display: inline-block;
  margin-left: 5px;
  margin-top: 5px;
  padding: 0;
  padding-left: 20px;
  position: relative;
  max-width: 100%;
  overflow: hidden;
  text-overflow: ellipsis;
  vertical-align: bottom;
  white-space: nowrap
}

.select2-container--default .select2-selection--multiple .select2-selection__choice__display {
  cursor: default;
  padding-left: 2px;
  padding-right: 5px
}

.select2-container--default .select2-selection--multiple .select2-selection__choice__remove {
  background-color: transparent;
  border: none;
  border-right: 1px solid #aaa;
  border-top-left-radius: 4px;
  border-bottom-left-radius: 4px;
  color: #999;
  cursor: pointer;
  font-size: 1em;
  font-weight: bold;
  padding: 0 4px;
  position: absolute;
  left: 0;
  top: 0
}

.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:hover,
.select2-container--default .select2-selection--multiple .select2-selection__choice__remove:focus {
  background-color: #f1f1f1;
  color: #333;
  outline: none
}

.select2-container--default[dir="rtl"] .select2-selection--multiple .select2-selection__choice {
  margin-left: 5px;
  margin-right: auto
}

.select2-container--default[dir="rtl"] .select2-selection--multiple .select2-selection__choice__display {
  padding-left: 5px;
  padding-right: 2px
}

.select2-container--default[dir="rtl"] .select2-selection--multiple .select2-selection__choice__remove {
  border-left: 1px solid #aaa;
  border-right: none;
  border-top-left-radius: 0;
  border-bottom-left-radius: 0;
  border-top-right-radius: 4px;
  border-bottom-right-radius: 4px
}

.select2-container--default[dir="rtl"] .select2-selection--multiple .select2-selection__clear {
  float: left;
  margin-left: 10px;
  margin-right: auto
}

.select2-container--default.select2-container--focus .select2-selection--multiple {
  border: solid black 1px;
  outline: 0
}

.select2-container--default.select2-container--disabled .select2-selection--multiple {
  background-color: #eee;
  cursor: default
}

.select2-container--default.select2-container--disabled .select2-selection__choice__remove {
  display: none
}

.select2-container--default.select2-container--open.select2-container--above .select2-selection--single,
.select2-container--default.select2-container--open.select2-container--above .select2-selection--multiple {
  border-top-left-radius: 0;
  border-top-right-radius: 0
}

.select2-container--default.select2-container--open.select2-container--below .select2-selection--single,
.select2-container--default.select2-container--open.select2-container--below .select2-selection--multiple {
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0
}

.select2-container--default .select2-search--dropdown .select2-search__field {
  border: 1px solid #aaa
}

.select2-container--default .select2-search--inline .select2-search__field {
  background: transparent;
  border: none;
  outline: 0;
  box-shadow: none;
  -webkit-appearance: textfield
}

.select2-container--default .select2-results>.select2-results__options {
  max-height: 200px;
  overflow-y: auto
}

.select2-container--default .select2-results__option .select2-results__option {
  padding-left: 1em
}

.select2-container--default .select2-results__option .select2-results__option .select2-results__group {
  padding-left: 0
}

.select2-container--default .select2-results__option .select2-results__option .select2-results__option {
  margin-left: -1em;
  padding-left: 2em
}

.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option {
  margin-left: -2em;
  padding-left: 3em
}

.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option {
  margin-left: -3em;
  padding-left: 4em
}

.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option {
  margin-left: -4em;
  padding-left: 5em
}

.select2-container--default .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option .select2-results__option {
  margin-left: -5em;
  padding-left: 6em
}

.select2-container--default .select2-results__option--group {
  padding: 0
}

.select2-container--default .select2-results__option--disabled {
  color: #999
}

.select2-container--default .select2-results__option--selected {
  background-color: #ddd
}

.select2-container--default .select2-results__option--highlighted.select2-results__option--selectable {
  background-color: #5897fb;
  color: white
}

.select2-container--default .select2-results__group {
  cursor: default;
  display: block;
  padding: 6px
}

.select2-container--classic .select2-selection--single {
  background-color: #f7f7f7;
  border: 1px solid #aaa;
  border-radius: 4px;
  outline: 0;
  background-image: -webkit-linear-gradient(top, #fff 50%, #eee 100%);
  background-image: -o-linear-gradient(top, #fff 50%, #eee 100%);
  background-image: linear-gradient(to bottom, #fff 50%, #eee 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#FFFFFFFF', endColorstr='#FFEEEEEE', GradientType=0)
}

.select2-container--classic .select2-selection--single:focus {
  border: 1px solid #5897fb
}

.select2-container--classic .select2-selection--single .select2-selection__rendered {
  color: #444;
  line-height: 28px
}

.select2-container--classic .select2-selection--single .select2-selection__clear {
  cursor: pointer;
  float: right;
  font-weight: bold;
  height: 26px;
  margin-right: 20px
}

.select2-container--classic .select2-selection--single .select2-selection__placeholder {
  color: #999
}

.select2-container--classic .select2-selection--single .select2-selection__arrow {
  background-color: #ddd;
  border: none;
  border-left: 1px solid #aaa;
  border-top-right-radius: 4px;
  border-bottom-right-radius: 4px;
  height: 26px;
  position: absolute;
  top: 1px;
  right: 1px;
  width: 20px;
  background-image: -webkit-linear-gradient(top, #eee 50%, #ccc 100%);
  background-image: -o-linear-gradient(top, #eee 50%, #ccc 100%);
  background-image: linear-gradient(to bottom, #eee 50%, #ccc 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#FFEEEEEE', endColorstr='#FFCCCCCC', GradientType=0)
}

.select2-container--classic .select2-selection--single .select2-selection__arrow b {
  border-color: #888 transparent transparent transparent;
  border-style: solid;
  border-width: 5px 4px 0 4px;
  height: 0;
  left: 50%;
  margin-left: -4px;
  margin-top: -2px;
  position: absolute;
  top: 50%;
  width: 0
}

.select2-container--classic[dir="rtl"] .select2-selection--single .select2-selection__clear {
  float: left
}

.select2-container--classic[dir="rtl"] .select2-selection--single .select2-selection__arrow {
  border: none;
  border-right: 1px solid #aaa;
  border-radius: 0;
  border-top-left-radius: 4px;
  border-bottom-left-radius: 4px;
  left: 1px;
  right: auto
}

.select2-container--classic.select2-container--open .select2-selection--single {
  border: 1px solid #5897fb
}

.select2-container--classic.select2-container--open .select2-selection--single .select2-selection__arrow {
  background: transparent;
  border: none
}

.select2-container--classic.select2-container--open .select2-selection--single .select2-selection__arrow b {
  border-color: transparent transparent #888 transparent;
  border-width: 0 4px 5px 4px
}

.select2-container--classic.select2-container--open.select2-container--above .select2-selection--single {
  border-top: none;
  border-top-left-radius: 0;
  border-top-right-radius: 0;
  background-image: -webkit-linear-gradient(top, #fff 0%, #eee 50%);
  background-image: -o-linear-gradient(top, #fff 0%, #eee 50%);
  background-image: linear-gradient(to bottom, #fff 0%, #eee 50%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#FFFFFFFF', endColorstr='#FFEEEEEE', GradientType=0)
}

.select2-container--classic.select2-container--open.select2-container--below .select2-selection--single {
  border-bottom: none;
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
  background-image: -webkit-linear-gradient(top, #eee 50%, #fff 100%);
  background-image: -o-linear-gradient(top, #eee 50%, #fff 100%);
  background-image: linear-gradient(to bottom, #eee 50%, #fff 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#FFEEEEEE', endColorstr='#FFFFFFFF', GradientType=0)
}

.select2-container--classic .select2-selection--multiple {
  background-color: white;
  border: 1px solid #aaa;
  border-radius: 4px;
  cursor: text;
  outline: 0;
  padding-bottom: 5px;
  padding-right: 5px
}

.select2-container--classic .select2-selection--multiple:focus {
  border: 1px solid #5897fb
}

.select2-container--classic .select2-selection--multiple .select2-selection__clear {
  display: none
}

.select2-container--classic .select2-selection--multiple .select2-selection__choice {
  background-color: #e4e4e4;
  border: 1px solid #aaa;
  border-radius: 4px;
  display: inline-block;
  margin-left: 5px;
  margin-top: 5px;
  padding: 0
}

.select2-container--classic .select2-selection--multiple .select2-selection__choice__display {
  cursor: default;
  padding-left: 2px;
  padding-right: 5px
}

.select2-container--classic .select2-selection--multiple .select2-selection__choice__remove {
  background-color: transparent;
  border: none;
  border-top-left-radius: 4px;
  border-bottom-left-radius: 4px;
  color: #888;
  cursor: pointer;
  font-size: 1em;
  font-weight: bold;
  padding: 0 4px
}

.select2-container--classic .select2-selection--multiple .select2-selection__choice__remove:hover {
  color: #555;
  outline: none
}

.select2-container--classic[dir="rtl"] .select2-selection--multiple .select2-selection__choice {
  margin-left: 5px;
  margin-right: auto
}

.select2-container--classic[dir="rtl"] .select2-selection--multiple .select2-selection__choice__display {
  padding-left: 5px;
  padding-right: 2px
}

.select2-container--classic[dir="rtl"] .select2-selection--multiple .select2-selection__choice__remove {
  border-top-left-radius: 0;
  border-bottom-left-radius: 0;
  border-top-right-radius: 4px;
  border-bottom-right-radius: 4px
}

.select2-container--classic.select2-container--open .select2-selection--multiple {
  border: 1px solid #5897fb
}

.select2-container--classic.select2-container--open.select2-container--above .select2-selection--multiple {
  border-top: none;
  border-top-left-radius: 0;
  border-top-right-radius: 0
}

.select2-container--classic.select2-container--open.select2-container--below .select2-selection--multiple {
  border-bottom: none;
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0
}

.select2-container--classic .select2-search--dropdown .select2-search__field {
  border: 1px solid #aaa;
  outline: 0
}

.select2-container--classic .select2-search--inline .select2-search__field {
  outline: 0;
  box-shadow: none
}

.select2-container--classic .select2-dropdown {
  background-color: #fff;
  border: 1px solid transparent
}

.select2-container--classic .select2-dropdown--above {
  border-bottom: none
}

.select2-container--classic .select2-dropdown--below {
  border-top: none
}

.select2-container--classic .select2-results>.select2-results__options {
  max-height: 200px;
  overflow-y: auto
}

.select2-container--classic .select2-results__option--group {
  padding: 0
}

.select2-container--classic .select2-results__option--disabled {
  color: grey
}

.select2-container--classic .select2-results__option--highlighted.select2-results__option--selectable {
  background-color: #3875d7;
  color: #fff
}

.select2-container--classic .select2-results__group {
  cursor: default;
  display: block;
  padding: 6px
}

.select2-container--classic.select2-container--open .select2-dropdown {
  border-color: #5897fb
}


@font-face {
  font-family: 'swiper-icons';
  src: url('data:application/font-woff;charset=utf-8;base64, d09GRgABAAAAAAZgABAAAAAADAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABGRlRNAAAGRAAAABoAAAAci6qHkUdERUYAAAWgAAAAIwAAACQAYABXR1BPUwAABhQAAAAuAAAANuAY7+xHU1VCAAAFxAAAAFAAAABm2fPczU9TLzIAAAHcAAAASgAAAGBP9V5RY21hcAAAAkQAAACIAAABYt6F0cBjdnQgAAACzAAAAAQAAAAEABEBRGdhc3AAAAWYAAAACAAAAAj//wADZ2x5ZgAAAywAAADMAAAD2MHtryVoZWFkAAABbAAAADAAAAA2E2+eoWhoZWEAAAGcAAAAHwAAACQC9gDzaG10eAAAAigAAAAZAAAArgJkABFsb2NhAAAC0AAAAFoAAABaFQAUGG1heHAAAAG8AAAAHwAAACAAcABAbmFtZQAAA/gAAAE5AAACXvFdBwlwb3N0AAAFNAAAAGIAAACE5s74hXjaY2BkYGAAYpf5Hu/j+W2+MnAzMYDAzaX6QjD6/4//Bxj5GA8AuRwMYGkAPywL13jaY2BkYGA88P8Agx4j+/8fQDYfA1AEBWgDAIB2BOoAeNpjYGRgYNBh4GdgYgABEMnIABJzYNADCQAACWgAsQB42mNgYfzCOIGBlYGB0YcxjYGBwR1Kf2WQZGhhYGBiYGVmgAFGBiQQkOaawtDAoMBQxXjg/wEGPcYDDA4wNUA2CCgwsAAAO4EL6gAAeNpj2M0gyAACqxgGNWBkZ2D4/wMA+xkDdgAAAHjaY2BgYGaAYBkGRgYQiAHyGMF8FgYHIM3DwMHABGQrMOgyWDLEM1T9/w8UBfEMgLzE////P/5//f/V/xv+r4eaAAeMbAxwIUYmIMHEgKYAYjUcsDAwsLKxc3BycfPw8jEQA/gZBASFhEVExcQlJKWkZWTl5BUUlZRVVNXUNTQZBgMAAMR+E+gAEQFEAAAAKgAqACoANAA+AEgAUgBcAGYAcAB6AIQAjgCYAKIArAC2AMAAygDUAN4A6ADyAPwBBgEQARoBJAEuATgBQgFMAVYBYAFqAXQBfgGIAZIBnAGmAbIBzgHsAAB42u2NMQ6CUAyGW568x9AneYYgm4MJbhKFaExIOAVX8ApewSt4Bic4AfeAid3VOBixDxfPYEza5O+Xfi04YADggiUIULCuEJK8VhO4bSvpdnktHI5QCYtdi2sl8ZnXaHlqUrNKzdKcT8cjlq+rwZSvIVczNiezsfnP/uznmfPFBNODM2K7MTQ45YEAZqGP81AmGGcF3iPqOop0r1SPTaTbVkfUe4HXj97wYE+yNwWYxwWu4v1ugWHgo3S1XdZEVqWM7ET0cfnLGxWfkgR42o2PvWrDMBSFj/IHLaF0zKjRgdiVMwScNRAoWUoH78Y2icB/yIY09An6AH2Bdu/UB+yxopYshQiEvnvu0dURgDt8QeC8PDw7Fpji3fEA4z/PEJ6YOB5hKh4dj3EvXhxPqH/SKUY3rJ7srZ4FZnh1PMAtPhwP6fl2PMJMPDgeQ4rY8YT6Gzao0eAEA409DuggmTnFnOcSCiEiLMgxCiTI6Cq5DZUd3Qmp10vO0LaLTd2cjN4fOumlc7lUYbSQcZFkutRG7g6JKZKy0RmdLY680CDnEJ+UMkpFFe1RN7nxdVpXrC4aTtnaurOnYercZg2YVmLN/d/gczfEimrE/fs/bOuq29Zmn8tloORaXgZgGa78yO9/cnXm2BpaGvq25Dv9S4E9+5SIc9PqupJKhYFSSl47+Qcr1mYNAAAAeNptw0cKwkAAAMDZJA8Q7OUJvkLsPfZ6zFVERPy8qHh2YER+3i/BP83vIBLLySsoKimrqKqpa2hp6+jq6RsYGhmbmJqZSy0sraxtbO3sHRydnEMU4uR6yx7JJXveP7WrDycAAAAAAAH//wACeNpjYGRgYOABYhkgZgJCZgZNBkYGLQZtIJsFLMYAAAw3ALgAeNolizEKgDAQBCchRbC2sFER0YD6qVQiBCv/H9ezGI6Z5XBAw8CBK/m5iQQVauVbXLnOrMZv2oLdKFa8Pjuru2hJzGabmOSLzNMzvutpB3N42mNgZGBg4GKQYzBhYMxJLMlj4GBgAYow/P/PAJJhLM6sSoWKfWCAAwDAjgbRAAB42mNgYGBkAIIbCZo5IPrmUn0hGA0AO8EFTQAA') format('woff');
  font-weight: 400;
  font-style: normal;
}

:root {
  --swiper-theme-color: #007aff;
}

.swiper-container {
  margin-left: auto;
  margin-right: auto;
  position: relative;
  overflow: hidden;
  list-style: none;
  padding: 0;
  /* Fix of Webkit flickering */
  z-index: 1;
}

.swiper-container-vertical>.swiper-wrapper {
  flex-direction: column;
}

.swiper-wrapper {
  position: relative;
  width: 100%;
  height: 100%;
  z-index: 1;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  transition-property: transform;
  box-sizing: content-box;
}

.swiper-container-android .swiper-slide,
.swiper-wrapper {
  transform: translate3d(0px, 0, 0);
}

.swiper-container-multirow>.swiper-wrapper {
  flex-wrap: wrap;
}

.swiper-container-multirow-column>.swiper-wrapper {
  flex-wrap: wrap;
  flex-direction: column;
}

.swiper-container-free-mode>.swiper-wrapper {
  transition-timing-function: ease-out;
  margin: 0 auto;
}

.swiper-container-pointer-events {
  touch-action: pan-y;
}

.swiper-container-pointer-events.swiper-container-vertical {
  touch-action: pan-x;
}

.swiper-slide {
  flex-shrink: 0;
  /* width: 100%;
  height: 100%; */
  display: inline-block !important;
  position: relative;
  transition-property: transform;
}

.swiper-slide-invisible-blank {
  visibility: hidden;
}

/* Auto Height */
.swiper-container-autoheight,
.swiper-container-autoheight .swiper-slide {
  height: auto;
}

.swiper-container-autoheight .swiper-wrapper {
  align-items: flex-start;
  transition-property: transform, height;
}

/* 3D Effects */
.swiper-container-3d {
  perspective: 1200px;
}

.swiper-container-3d .swiper-wrapper,
.swiper-container-3d .swiper-slide,
.swiper-container-3d .swiper-slide-shadow-left,
.swiper-container-3d .swiper-slide-shadow-right,
.swiper-container-3d .swiper-slide-shadow-top,
.swiper-container-3d .swiper-slide-shadow-bottom,
.swiper-container-3d .swiper-cube-shadow {
  transform-style: preserve-3d;
}

.swiper-container-3d .swiper-slide-shadow-left,
.swiper-container-3d .swiper-slide-shadow-right,
.swiper-container-3d .swiper-slide-shadow-top,
.swiper-container-3d .swiper-slide-shadow-bottom {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 10;
}

.swiper-container-3d .swiper-slide-shadow-left {
  background-image: linear-gradient(to left, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}

.swiper-container-3d .swiper-slide-shadow-right {
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}

.swiper-container-3d .swiper-slide-shadow-top {
  background-image: linear-gradient(to top, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}

.swiper-container-3d .swiper-slide-shadow-bottom {
  background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0));
}

/* CSS Mode */
.swiper-container-css-mode>.swiper-wrapper {
  overflow: auto;
  scrollbar-width: none;
  /* For Firefox */
  -ms-overflow-style: none;
  /* For Internet Explorer and Edge */
}

.swiper-container-css-mode>.swiper-wrapper::-webkit-scrollbar {
  display: none;
}

.swiper-container-css-mode>.swiper-wrapper>.swiper-slide {
  scroll-snap-align: start start;
}

.swiper-container-horizontal.swiper-container-css-mode>.swiper-wrapper {
  scroll-snap-type: x mandatory;
}

.swiper-container-vertical.swiper-container-css-mode>.swiper-wrapper {
  scroll-snap-type: y mandatory;
}

:root {
  --swiper-navigation-size: 44px;
  /*
  --swiper-navigation-color: var(--swiper-theme-color);
  */
}

.swiper-button-prev,
.swiper-button-next {
  position: absolute;
  top: 50%;
  z-index: 10;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}

.swiper-button-prev.swiper-button-disabled,
.swiper-button-next.swiper-button-disabled {
  opacity: 0.7;
  cursor: auto;
  pointer-events: none;
}

.swiper-button-prev:after,
.swiper-button-next:after {
  font-family: swiper-icons;
  text-transform: none !important;
  letter-spacing: 0;
  text-transform: none;
  font-variant: initial;
  line-height: 1;
}

.swiper-button-prev,
.swiper-container-rtl .swiper-button-next {
  left: 10px;
  right: auto;
}

.swiper-button-prev:after,
.swiper-container-rtl .swiper-button-next:after {
  content: 'prev';
}

.swiper-button-next,
.swiper-container-rtl .swiper-button-prev {
  right: 10px;
  left: auto;
}

.swiper-button-next:after,
.swiper-container-rtl .swiper-button-prev:after {
  content: 'next';
}

.swiper-button-prev.swiper-button-white,
.swiper-button-next.swiper-button-white {
  --swiper-navigation-color: #ffffff;
}

.swiper-button-prev.swiper-button-black,
.swiper-button-next.swiper-button-black {
  --swiper-navigation-color: #000000;
}

.swiper-button-lock {
  display: none;
}

:root {
  /*
  --swiper-pagination-color: var(--swiper-theme-color);
  */
}

.swiper-pagination {
  position: absolute;
  text-align: center;
  transition: 300ms opacity;
  transform: translate3d(0, 0, 0);
  z-index: 10;
}

.swiper-pagination.swiper-pagination-hidden {
  opacity: 0;
}

/* Common Styles */
.swiper-pagination-fraction,
.swiper-pagination-custom,
.swiper-container-horizontal>.swiper-pagination-bullets {
  bottom: 10px;
  left: 0;
  width: 100%;
}

/* Bullets */
.swiper-pagination-bullets-dynamic {
  overflow: hidden;
  font-size: 0;
}

.swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  transform: scale(0.33);
  position: relative;
}

.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active {
  transform: scale(1);
}

.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-main {
  transform: scale(1);
}

.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-prev {
  transform: scale(0.66);
}

.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-prev-prev {
  transform: scale(0.33);
}

.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-next {
  transform: scale(0.66);
}

.swiper-pagination-bullets-dynamic .swiper-pagination-bullet-active-next-next {
  transform: scale(0.33);
}

.swiper-pagination-bullet {
  width: 8px;
  height: 8px;
  display: inline-block;
  border-radius: 50%;
  background: #000;
  opacity: 0.2;
}

button.swiper-pagination-bullet {
  border: none;
  margin: 0;
  padding: 0;
  box-shadow: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
}

.swiper-pagination-clickable .swiper-pagination-bullet {
  cursor: pointer;
}

.swiper-pagination-bullet-active {
  opacity: 1;
  background: var(--swiper-pagination-color, var(--swiper-theme-color));
}

.swiper-container-vertical>.swiper-pagination-bullets {
  right: 10px;
  top: 50%;
  transform: translate3d(0px, -50%, 0);
}

.swiper-container-vertical>.swiper-pagination-bullets .swiper-pagination-bullet {
  margin: 6px 0;
  display: block;
}

.swiper-container-vertical>.swiper-pagination-bullets.swiper-pagination-bullets-dynamic {
  top: 50%;
  transform: translateY(-50%);
  width: 8px;
}

.swiper-container-vertical>.swiper-pagination-bullets.swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  display: inline-block;
  transition: 200ms transform, 200ms top;
}

.swiper-container-horizontal>.swiper-pagination-bullets .swiper-pagination-bullet {
  margin: 0 4px;
}

.swiper-container-horizontal>.swiper-pagination-bullets.swiper-pagination-bullets-dynamic {
  left: 50%;
  transform: translateX(-50%);
  white-space: nowrap;
}

.swiper-container-horizontal>.swiper-pagination-bullets.swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  transition: 200ms transform, 200ms left;
}

.swiper-container-horizontal.swiper-container-rtl>.swiper-pagination-bullets-dynamic .swiper-pagination-bullet {
  transition: 200ms transform, 200ms right;
}

/* Progress */
.swiper-pagination-progressbar {
  background: rgba(0, 0, 0, 0.25);
  position: absolute;
}

.swiper-pagination-progressbar .swiper-pagination-progressbar-fill {
  background: var(--swiper-pagination-color, var(--swiper-theme-color));
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  transform: scale(0);
  transform-origin: left top;
}

.swiper-container-rtl .swiper-pagination-progressbar .swiper-pagination-progressbar-fill {
  transform-origin: right top;
}

.swiper-container-horizontal>.swiper-pagination-progressbar,
.swiper-container-vertical>.swiper-pagination-progressbar.swiper-pagination-progressbar-opposite {
  width: 100%;
  height: 4px;
  left: 0;
  top: 0;
}

.swiper-container-vertical>.swiper-pagination-progressbar,
.swiper-container-horizontal>.swiper-pagination-progressbar.swiper-pagination-progressbar-opposite {
  width: 4px;
  height: 100%;
  left: 0;
  top: 0;
}

.swiper-pagination-white {
  --swiper-pagination-color: #ffffff;
}

.swiper-pagination-black {
  --swiper-pagination-color: #000000;
}

.swiper-pagination-lock {
  display: none;
}

/* Scrollbar */
.swiper-scrollbar {
  border-radius: 10px;
  position: relative;
  -ms-touch-action: none;
  background: rgba(0, 0, 0, 0.1);
}

.swiper-container-horizontal>.swiper-scrollbar {
  position: absolute;
  left: 1%;
  bottom: 3px;
  z-index: 50;
  height: 5px;
  width: 98%;
}

.swiper-container-vertical>.swiper-scrollbar {
  position: absolute;
  right: 3px;
  top: 1%;
  z-index: 50;
  width: 5px;
  height: 98%;
}

.swiper-scrollbar-drag {
  height: 100%;
  width: 100%;
  position: relative;
  background: rgba(0, 0, 0, 0.5);
  border-radius: 10px;
  left: 0;
  top: 0;
}

.swiper-scrollbar-cursor-drag {
  cursor: move;
}

.swiper-scrollbar-lock {
  display: none;
}

.swiper-zoom-container {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.swiper-zoom-container>img,
.swiper-zoom-container>svg,
.swiper-zoom-container>canvas {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}

.swiper-slide-zoomed {
  cursor: move;
}

/* Preloader */


.swiper-lazy-preloader {
  width: 42px;
  height: 42px;
  position: absolute;
  left: 50%;
  top: 50%;
  margin-left: -21px;
  margin-top: -21px;
  z-index: 10;
  transform-origin: 50%;
  animation: swiper-preloader-spin 1s infinite linear;
  box-sizing: border-box;
  border: 4px solid var(--swiper-preloader-color, var(--swiper-theme-color));
  border-radius: 50%;
  border-top-color: transparent;
}

.swiper-lazy-preloader-white {
  --swiper-preloader-color: #fff;
}

.swiper-lazy-preloader-black {
  --swiper-preloader-color: #000;
}

@keyframes swiper-preloader-spin {
  100% {
    transform: rotate(360deg);
  }
}

/* a11y */
.swiper-container .swiper-notification {
  position: absolute;
  left: 0;
  top: 0;
  pointer-events: none;
  opacity: 0;
  z-index: -1000;
}

.swiper-container-fade.swiper-container-free-mode .swiper-slide {
  transition-timing-function: ease-out;
}

.swiper-container-fade .swiper-slide {
  pointer-events: none;
  transition-property: opacity;
}

.swiper-container-fade .swiper-slide .swiper-slide {
  pointer-events: none;
}

.swiper-container-fade .swiper-slide-active,
.swiper-container-fade .swiper-slide-active .swiper-slide-active {
  pointer-events: auto;
}

.swiper-container-cube {
  overflow: visible;
}

.swiper-container-cube .swiper-slide {
  pointer-events: none;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
  z-index: 1;
  visibility: hidden;
  transform-origin: 0 0;
  width: 100%;
  height: 100%;
}

.swiper-container-cube .swiper-slide .swiper-slide {
  pointer-events: none;
}

.swiper-container-cube.swiper-container-rtl .swiper-slide {
  transform-origin: 100% 0;
}

.swiper-container-cube .swiper-slide-active,
.swiper-container-cube .swiper-slide-active .swiper-slide-active {
  pointer-events: auto;
}

.swiper-container-cube .swiper-slide-active,
.swiper-container-cube .swiper-slide-next,
.swiper-container-cube .swiper-slide-prev,
.swiper-container-cube .swiper-slide-next+.swiper-slide {
  pointer-events: auto;
  visibility: visible;
}

.swiper-container-cube .swiper-slide-shadow-top,
.swiper-container-cube .swiper-slide-shadow-bottom,
.swiper-container-cube .swiper-slide-shadow-left,
.swiper-container-cube .swiper-slide-shadow-right {
  z-index: 0;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

.swiper-container-cube .swiper-cube-shadow {
  position: absolute;
  left: 0;
  bottom: 0px;
  width: 100%;
  height: 100%;
  opacity: 0.6;
  z-index: 0;
}

.swiper-container-cube .swiper-cube-shadow:before {
  content: '';
  background: #000;
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  -webkit-filter: blur(50px);
  filter: blur(50px);
}

.swiper-container-flip {
  overflow: visible;
}

.swiper-container-flip .swiper-slide {
  pointer-events: none;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
  z-index: 1;
}

.swiper-container-flip .swiper-slide .swiper-slide {
  pointer-events: none;
}

.swiper-container-flip .swiper-slide-active,
.swiper-container-flip .swiper-slide-active .swiper-slide-active {
  pointer-events: auto;
}

.swiper-container-flip .swiper-slide-shadow-top,
.swiper-container-flip .swiper-slide-shadow-bottom,
.swiper-container-flip .swiper-slide-shadow-left,
.swiper-container-flip .swiper-slide-shadow-right {
  z-index: 0;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}
</style>
