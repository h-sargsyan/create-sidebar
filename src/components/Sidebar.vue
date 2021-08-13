<template>
  <div class="sidebar">

		<!-- Carousel -->
		<div class="carousel">
			<Carousel />
		</div>
		<!-- / Carousel -->

		<div class="sidebar_main">

			<!-- Main Header -->
			<div class="main_header">
				<div class="main_header_title">
					<h5>ID 64648</h5>
					<p>Նորակառույց</p>
				</div>
				<div class="main_header_body">
					<p class="main_header_data">20.01.2020</p>
					<p class="main_header_sale">Վաճառվում է առանձնատուն</p>
					<p><img src="../assets/logos/gps.png" alt="">Amiryan-10, Amiryan Street, Yerevan</p>
					<a href="#"><span id="wrong_address">Սխալ հասցե ?</span></a>
				</div>
			</div>
			<!-- / Main Header -->

			<!-- Sidebar Sale -->
			<div class="sidebar_sale">
				<div class="sale_price">
					<h3>Գինը՝</h3>
					<span id="price">120.000 $</span>
				</div>
				<div class="sale_rent">
					<div class="rent_monthly">
						<p>Ամսավարձ\</p>
						<span id="rent_monthly_price">85.000 ֏</span>
					</div>
					<div class="rent_daily">
						<p>Օրավարձ\</p>
						<span id="rent_daily_price">15.000 ֏</span>
					</div>
				</div>
			</div>
			<!-- / Sidebar Sale -->

			<!-- Sidebar About -->
			<div class="sidebar_about">
				<div class="holder" :class="{'text_hide': textShowHide, 'text_show': !textShowHide}">
					<div class="limited l-200">
						<h4>Նկարագրություն</h4>
						<p>
							Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut nec ultrices magna. Etiam sollicitudin mi quis aliquet cursus. Donec faucibus volutpat finibus. Praesent vitae ex ornare, pharetra metus eu, maximus dolor. Maecenas placerat bibendum efficitur. Fusce non feugiat urna. Maecenas id volutpat massa, et<span :class="{'hideBtn': textShowHide}" id="more">...</span><button class="moreBtn" type="button" @click="textShowHide = !textShowHide" :class="{'hideBtn': textShowHide}">Կարդալ ավելին</button><span>maximus velit. Quisque congue tellus non augue ornare, et gravida tortor pretium. Lorem ipsum dolor consectetur adipiscing elit. Ut nec ultrices magna. Etiam sollicitudin mi quis aliquet cursus. Donec faucibus volutpat finibus. Praesent vitae ex ornare, pharetra metus eu, maximus dolor. Maecenas placerat bibendum efficitur. Fusce non feugiat urna. Maecenas id volutpat massa, et maximus velit. Quisque congue tellus non augue ornare, et gravida tortor pretium.</span>
							<button class="moreBtn" type="button" @click="textShowHide = !textShowHide">Փակել</button>
						</p>
					</div>
				</div>
			</div>
			<!-- / Sidebar About -->

			<!-- Sidebar Geometries -->
			<div class="sidebar_geometries">
				<div class="geometries_stairs">
					<img src="../assets/logos/stairs.png" alt="">
					<span id="stairs_count">3</span>
				</div>
				<div class="geometries_area">
					<img src="../assets/logos/area.png" alt="">
					<span id="area_count">120 քմ</span>
				</div>
				<div class="geometries_bed">
					<img src="../assets/logos/bed.png" alt="">
					<span id="stairs_count">3</span>
				</div>
				<div class="geometries_info">
					<a href="#"><img src="../assets/logos/info.png" alt=""></a>
				</div>
			</div>
			<!-- / Sidebar Geometries -->

			<!-- Sidebar About Home -->
			<div class="sidebar_about_home">
				<div class="about_home_title">
					<h5>Շենքի հարկերի քանակ - </h5>
					<p>10</p>
				</div>
				<div class="about_home_title">
					<h5>Բնակարանի հարկ - </h5>
					<p>7</p>
				</div>
				<div class="about_home_title">
					<h5>Սանհանգույցների քանակը - </h5>
					<p>2</p>
				</div>
				<div class="about_home_title">
					<h5>Սեփականության վիճակը - </h5>
					<p>Գերազանց</p>
				</div>
				<div class="about_home_title">
					<h5>Սեփականության տիպը - </h5>
					<p>Քարե</p>
				</div>
			</div>
			<!-- / Sidebar About Home -->

			<!-- Sidebar Communals -->
			<div class="sidebar_communals" :class="{'hide_text': !hideText, 'show_text': hideText}">
				<div class="communals_title">
					<h5>Կոմունալ հարմարություններ</h5>
					<button
					type="button"
					class="btn_"
					:class="{'transform': !hideText}"
					@click="hideText = !hideText">
						<img id="arrow" src="../assets/logos/arrow.png"
						alt="">
					</button>
				</div>
				<div class="communals_info">
					<span id="communals_tags">Ջեռուցում / Գազ / Տաք ջուր / Էլեկտրաէներգիա/ Մշտական ջուր / Խմելու ջուր / Ինտերնետ</span>
				</div>
			</div>
			<!-- / Sidebar Communals -->

			<!-- Sidebar other -->
			<div class="sidebar_other" :class="{'hide_text': !hideTextOther, 'show_text': hideTextOther}">
				<div class="other_title">
					<h5>Այլ</h5>
					<button type="button"
					class="btn_2"
					:class="{'transform': !hideTextOther}"
					@click="hideTextOther = !hideTextOther">
						<img id="arrow" src="../assets/logos/arrow.png"
						alt="">
					</button>
				</div>
				<div class="other_info">
					<span id="other_tags">Բաց պատշգամբ / Ավտոկայանատեղի / Վանդակաճաղեր</span>
				</div>
			</div>
			<!-- / Sidebar Other -->

			<!-- Sidebar Footer -->
			<div class="sidebar_footer">
				<div class="account_body">
					<div class="account_info">
						<img src="../assets/logos/account.png" alt="">
						<div class="account_name">
							<p>Անահիտ Պողոսյան</p>
							<span class="account_role">Անհատ</span>
						</div>
					</div>
					<div class="account_alert">
						<a href="#"><img src="../assets/logos/alert.png" alt=""></a>
					</div>
				</div>
				<div class="footer_buttons">
					<button type="button" id="send_message">Գրել Նամակ</button>
					<button type="button" id="call">Զանգահարել</button>
				</div>
			</div>
			<!-- / Sidebar Footer -->
		</div>
	</div>
</template>

<script>
import Carousel from './Carousel/Carousel.vue'

export default {
	data () {
		return {
			hideText: true,
			hideTextOther: true,
			textShowHide: false
		}
	},
	components: {
		Carousel
	},
	methods: {
		hideBtn () {
			document.querySelector('#more', '#moreBtn').style.display = 'none'
			console.log('ok')
		}
	}
}
</script>

<style scoped>
.sidebar {
	width: 460px;
	margin-left: 50px;
	margin-top: 15px;
	font-size: 14px;
	box-shadow: -2px 0 14px 0 rgba(0, 0, 0, 0.36);
	padding: 0 0 29px;
}
.carousel {
	height: 288px;
	background-color: teal;
}

/* Start Sidebar Main Styles */
.sidebar_main {
	width: 416px;
	height: 100%;
	margin: 24px auto 0;
}

.main_header {
	width: 100%;
	height: 100%;
	padding-bottom: 16px;
	border-bottom: 1px solid silver;
}

.main_header_title {
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.main_header_title h5 {
	font-size: 18px;
	font-weight: normal;
}

.main_header_title p {
	background-color: rgba(255,147,18, 0.41);
	padding: 5px 15px;
  border-radius: 5px;
}

.main_header_body {
	width: 100%;
	height: 100%;
	margin-top: 8px;
}

.main_header_body p{
	color: rgba(1,3,2, 0.48);
	margin-bottom: 8px;
}

.main_header_body p img {
	margin-right: 8px;
}

#wrong_address {
	color: #e91d46;
}
/* END Sidebar Main Styles*/

/* Start Sidebar Sale Styles */
.sidebar_sale {
	width: 100%;
	height: 100%;
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin-top: 19px;
	border-bottom: 1px solid silver;
	padding-bottom: 18px;
}

.sidebar_sale span {
	color: #04a777;
}

.sale_price {
	display: flex;
	justify-content: space-between;
	align-items: center;
	width: 162px;
}

.sale_price h3 {
	font-size: 16px;
  font-weight: bold;
}

#price {
	font-size: 24px;
  font-weight: 600;
}

.sale_rent {
	width: 198px;
	height: 100%;
}

.sale_rent span {
	color: #04a777;
	font-size: 17px;
  font-weight: 600;
}

.rent_monthly, .rent_daily {
	width: 100%;
	display: flex;
	justify-content: space-between;
	align-items: center;
}

.rent_monthly {
	margin-bottom: 8px;
}

.rent_daily p {
	padding: 0 8px;
}
/* END Sidebar Sale Styles */

/* Start Sidebar About Styles */
.sidebar_about {
	font-size: 16px;
	margin-top: 16px;
	border-bottom: 1px solid silver;
	padding-bottom: 16px;
}
.sidebar_about h4 {
	font-weight: bold;
	margin-bottom: 16px;
}
.text_hide {
	animation-name: hide-text;
	animation-duration: .3s;
	animation-fill-mode: forwards;
}
@keyframes hide-text {
	0% {
		height: 144px;
		overflow: hidden;
	}
	100% {
		height: 288px;
		overflow: hidden;
	}
}

.text_show {
	animation-name: show-text;
	animation-duration: .3s;
	animation-fill-mode: forwards;
}
@keyframes show-text {
	0% {
		height: 288px;
		overflow: hidden;
	}
	100% {
		height: 144px;
		overflow: hidden;
	}
}
.hideBtn {
	display: none;
}

.moreBtn {
	border: none;
	font-size: 16px;
	background: transparent;
	color: #04a777;
	cursor: pointer;
	margin-left: 5px;
}
/* END Sidebar About Styles */

/* Start Sidebar Geometries Styles */
.sidebar_geometries {
	width: 100%;
	height: 100%;
	display: flex;
	margin: 16px 0;
	border-bottom: 1px solid silver;
	padding-bottom: 16px;
}

.geometries_stairs, .geometries_area, .geometries_bed {
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin-right: 37px;
}
.geometries_bed {
	margin-right: 5px;
}

.geometries_info {
	margin-top: 3px;
}

.geometries_stairs img, .geometries_area img, .geometries_bed img {
	margin-right: 17px;
}
/* END Sidebar Geometries Styles */

/* Start Sidebar About Home Styles */
.sidebar_about_home {
	width: 100%;
	height: 100%;
	border-bottom: 1px solid silver;
	font-size: 16px;
}

.about_home_title {
	display: flex;
	margin-bottom: 16px;
}

.about_home_title h5 {
	font-weight: bold;
}

.about_home_title p {
	margin-left: 3px;
}
/* END Sidebar About Home Styles */

/* Start Sidebar Communals and Sidebar Other Styles */
.sidebar_communals, .sidebar_other {
	width: 100%;
	height: 100%;
	margin-top: 16px;
	padding-bottom: 16px;
	border-bottom: 1px solid silver;
	font-size: 16px;
	transition: .3s;
	animation-name: show;
}

.communals_title, .other_title {
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin-bottom: 16px;
}

.communals_title h5, .other_title h5 {
	font-weight: bold;
	line-height: 1.38;
}

.other_info span {
	font-size: 14px;
}

.btn_, .btn_2 {
	padding: 0 5px;
	border: none;
	background: transparent;
	cursor: pointer;
}

.hide_text {
	animation-name: hide;
	animation-duration: .3s;
	animation-fill-mode: forwards;
}
@keyframes hide {
	0% {
		height: 70px;
	}
	100% {
		height: 15px;
		overflow: hidden;
	}
}

.transform {
	transform: rotate(180deg);
}

.show_text {
	animation-name: show;
	animation-duration: .3s;
	animation-fill-mode: forwards;
}
@keyframes show {
	0% {
		height: 15px;
		overflow: hidden;
	}
	100% {
		height: 70px;
	}
}
/* End Sidebar Communals and Sidebar Other Styles */

/* Start Sidebar Footer Styles */
.sidebar_footer {
	width: 100%;
	height: 100%;
	margin-top: 16px;
}

.account_body {
	width: 100%;
	height: 100%;
	display: flex;
	justify-content: space-between;
}

.account_info {
	display: flex;
}
.account_info img {
	width: 32px;
	height: 32px;
	margin-right: 16px;
}

.account_name p {
	margin-bottom: 5px;
	font-size: 16px;
}

#account_role {
	font-size: 14px;
}

.footer_buttons {
	width: 100%;
	height: 100%;
	display: flex;
	justify-content: space-between;
	align-items: center;
	margin-top: 16px;
}

.footer_buttons button {
	border: none;
	border-radius: 5px;
	color: #fff;
	cursor: pointer;
	font-size: 16px;
}

#send_message {
	padding: 9px 45px;
	background-color: #ff9312;
}
#send_message:hover {
	background-color: #e98b17;
}
#call {
	padding: 9px 45px;
	background-color: #04a777;
}
#call:hover {
	background-color: #09946a;
}
/* End Sidebar Footer Styles */

</style>