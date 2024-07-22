<script setup>

import { onMounted } from 'vue'

onMounted(() => {     

	$('.homepage-slides').owlCarousel({
		items: 1,
		dots: false,
		nav: true,
		loop: true,
		autoplay: true,
		autoplayTimeout: 5000,
		smartSpeed: 2000,
		slideSpeed: 600,
		animateOut: 'fadeOut',
		navText: ["<i class='la la-angle-left'></i>", "<i class='la la-angle-right'></i>"],
		responsive: {
			0: {
				items: 1,
				nav: false,
				dots: false,
			},
			600: {
				items: 1,
				nav: false,
				dots: false,
			},
			768: {
				items: 1,
				nav: false,
				dots: false,
			},
			1100: {
				items: 1,
				nav: true,
				dots: false,
			}
		}
	});


	$(".homepage-slides").on("translate.owl.carousel", function () {
		$(".single-slide-item h1").removeClass("animated fadeInUp").css("opacity", "1");
		$(".single-slide-item h6").removeClass("animated fadeInDown").css("opacity", "1");
		$(".single-slide-item p").removeClass("animated fadeInDown").css("opacity", "1");
		$(".single-slide-item a.main-btn").removeClass("animated fadeInDown").css("opacity", "1");
	});

	$(".homepage-slides").on("translated.owl.carousel", function () {
		$(".single-slide-item h1").addClass("animated fadeInUp").css("opacity", "1");
		$(".single-slide-item h6").addClass("animated fadeInDown").css("opacity", "1");
		$(".single-slide-item p").addClass("animated fadeInDown").css("opacity", "1");
		$(".single-slide-item a.main-btn").addClass("animated fadeInDown").css("opacity", "1");
	});
  
});

</script>

<template>
	<div class="single-slide-item hero-area-bg-2">
	  <div></div>
	  <div>
		<div class="container">
		  <div>
			<div class="col-lg-12 wow fadeInUp animated" data-wow-delay=".2s">
			  <div class="image-container">
				<img src="/assets/img/robo.png" alt="">
			  </div>
			  <div>
				<h1>Impulsa Tus Ventas</h1>
				<h3 class="negro">Lleva Tu Negocio Al Siguiente Nivel</h3>
				<p class="negro">Lorem, ipsum dolor sit amet consectetur adipisicing elit. ipsum dolor sit amet consectetur adipisicing elit     </p>
				<!---p class="negro">ipsum dolor sit amet consectetur adipisicing elit</p> -->
			  </div>
			  <!---router-link :to="{name:'about'}" class="main-btn">Learn More</router-link> ---->
			  <button class="custom-button">Regístrate</button>
			</div>
		  </div>
		</div>
	  </div>
	</div>
  </template>
  
  <style scoped>
  .negro {
	color: black;
	margin-top: 0;
  }
  
  .image-container {
	width: 40%;
	float: right;
	margin-left: 20px;
  }
  .custom-button {
	width: 15%;
  background-color: white;
  color: black;
  border: 2px solid #1e90ff;;
  padding: 10px 20px; /* Ajusta el tamaño del botón */
  font-size: 16px; /* Ajusta el tamaño del texto */
  border-radius: 5px; /* Opcional: para bordes redondeados */
  cursor: pointer; /* Cambia el cursor al pasar sobre el botón */
}

.custom-button:hover {
  background-color: #1e90ff;;
  color: white;
}
  </style>