<script setup>
	import { ref } from "vue"
	// Import Swiper Vue.js components
	import { Swiper, SwiperSlide } from "swiper/vue"

	import "swiper/css"

	// import required modules
	import { FreeMode, Navigation, Thumbs } from "swiper/modules"

	const thumbsSwiper = ref(null)

	const setThumbsSwiper = (swiper) => {
		thumbsSwiper.value = swiper
	}

	var swiper = new Swiper(".mySwiper", {
		loop: true,
		spaceBetween: 10,
		slidesPerView: 4,
		freeMode: true,
		watchSlidesProgress: true,
	})
	var swiper2 = new Swiper(".mySwiper2", {
		loop: true,
		spaceBetween: 10,
		navigation: {
			nextEl: ".swiper-button-next",
			prevEl: ".swiper-button-prev",
		},
		thumbs: {
			swiper: swiper,
		},
	})
</script>
<template>
	<section>
		<div style="--swiper-navigation-color: #fff; --swiper-pagination-color: #fff" class="swiper mySwiper2">
			<div class="swiper-wrapper">
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-1.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-2.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-3.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-4.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-5.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-6.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-7.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-8.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-9.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-10.jpg" />
				</div>
			</div>
			<div class="swiper-button-next"></div>
			<div class="swiper-button-prev"></div>
		</div>
		<div thumbsSlider="" class="swiper mySwiper">
			<div class="swiper-wrapper">
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-1.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-2.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-3.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-4.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-5.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-6.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-7.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-8.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-9.jpg" />
				</div>
				<div class="swiper-slide">
					<img src="https://swiperjs.com/demos/images/nature-10.jpg" />
				</div>
			</div>
		</div>
	</section>
</template>
