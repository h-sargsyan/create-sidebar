<template>
	<div class="carousel_body">
		<splide>
			<splide-slide>
				<img src="https://picsum.photos/id/237/600/300">
			</splide-slide>
			<splide-slide>
				<img src="https://picsum.photos/id/236/600/300">
			</splide-slide>
			<splide-slide>
				<img src="https://picsum.photos/id/235/600/300">
			</splide-slide>
			<splide-slide>
				<img src="https://picsum.photos/id/234/600/300">
			</splide-slide>
			<splide-slide>
				<img src="https://picsum.photos/id/233/600/300">
			</splide-slide>
		</splide>
		<div class="slide_options">
			<button type="button" class="btn_options"><img src="../../assets/logos/tack.png" alt=""></button>
			<button type="button" class="btn_options"><img src="../../assets/logos/share.png" alt=""></button>
			<button type="button" class="btn_options"><img src="../../assets/logos/close.png" alt=""></button>
		</div>
		<div class="image_count">
			<span id="image_count">11</span>
			<img src="../../assets/logos/image.png" alt="">
		</div>
	</div>
</template>

<script>
import { Splide, SplideSlide } from '@splidejs/vue-splide'
import '@splidejs/splide/dist/css/splide.min.css/'
export default {
	data () {
		return {
			options: {
				rewind: true,
				width: 800,
				gap: '1rem'
			}
		}
	},
	components: {
		Splide, SplideSlide
	}
}
</script>

<style scoped>
.splide {
	width: 100%;
	height: 100%;
}

.splide__slide {
	width: 460px;
	height: 288px;
}

.splide__slide img {
	object-fit: cover;
	width: 100%;
	height: 100%;
}

.carousel_body {
	position: relative;
}

.slide_options {
	position: absolute;
	top: 16px;
	right: 16px;
	width: 115px;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.btn_options {
	background-color: transparent;
	border: none;
	cursor: pointer;
}

.image_count{
	background-color: rgba(1,3,2, 0.48);
	width: 38px;
	height: 22px;
	padding: 4px 12px 5px 12px;
  border-radius: 24px;
	position: absolute;
	bottom: 16px;
	right: 16px;
	font-size: 14px;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.image_count span {
	color: #fff;
}

</style>
