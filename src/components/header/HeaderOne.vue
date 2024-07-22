<script setup>

</script>

<template>
	<h1></h1>
    <header class="header-area">
 		<div class="sticky-area">
 			<div class="navigation">
 				<div class="container">
 					<div class="row align-items-center">
 						<div class="col-lg-3">
							<router-link class="navbar-brand" to="/"><img class="imagen" src="/assets/img/logo-black.png" alt=""></router-link>
 							<!--div class="logo">
 							</div> -->
 						</div>
 						<div class="col-lg-6">
 							<div class="main-menu">
 								<nav class="navbar navbar-expand-lg">
 									<!---button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
 										<span class="navbar-toggler-icon"></span>
 										<span class="navbar-toggler-icon"></span>
 										<span class="navbar-toggler-icon"></span>
 									</button> --->

 									<div class="collapse navbar-collapse justify-content-center" id="navbarSupportedContent">
 										<ul >
 											<li class="nav-item">
												<a class="nav-link" href="#">Lorem
 													<span class="sub-nav-toggler">
 													</span>
 												</a>
 												<!---ul class="sub-menu">
 													<li><router-link :to="{name:'home'}">Home-Main</router-link></li>
 													<li><router-link :to="{name:'home2'}">Home-Industry</router-link></li>
 													<li><router-link :to="{name:'home3'}">Home-Construction</router-link></li>
 												</ul> --->
 											</li>

 											<li class="nav-item">
 												<a class="nav-link" href="#">Impsum
 													<span class="sub-nav-toggler">
 													</span>
 												</a>
 												<!--ul class="sub-menu">
 													<li><router-link :to="{name:'about'}">About us</router-link></li>
 													<li><router-link :to="{name:'choose-us'}">Why Choose Us</router-link></li>
 													<li><router-link :to="{name:'team'}">Our Team</router-link></li>
 													<li><router-link :to="{name:'price'}">Pricing</router-link></li>
 													<li><router-link :to="{name:'faq'}">FAQ</router-link></li>
 												</ul> --->
 											</li>
 											<li class="nav-item">
 												<a class="nav-link" href="#">Dolor
 													<span class="sub-nav-toggler">
 													</span>
 												</a>
 												<!--ul class="sub-menu">
 													<li><router-link :to="{name:'service-1'}">Services-01</router-link></li>
 													<li><router-link :to="{name:'service-2'}">Services-02</router-link></li>
 													<li><router-link :to="{name:'service-details'}">Service Details</router-link></li>
 												</ul> -->

 											</li>

 											<li class="nav-item">
 												<a class="nav-link" href="#">Sit
 													<span class="sub-nav-toggler">
 													</span>
 												</a>
 												<!--ul class="sub-menu">
 													<li><router-link :to="{name:'project'}">Projects</router-link></li>
 													<li><router-link :to="{name:'project-details'}">Project Details</router-link></li>
 												</ul> -->
 											</li>

 											<!-----li class="nav-item">
 												<a class="nav-link" href="#">Blog
 													<span class="sub-nav-toggler">
 													</span>
 												</a>
 												<ul class="sub-menu">
 													<li><router-link :to="{name:'blog'}">Blog</router-link></li>
 													<li><router-link :to="{name:'blog-details'}">Blog Details</router-link></li>
 												</ul>
 											</li>
 											<li class="nav-item">
 												<router-link class="nav-link" :to="{name:'contact'}">Contact</router-link>
 											</li> --->
 										</ul>

 									</div>
 								</nav>
 							</div>
 						</div>
 						<div class="col-lg-3 text-end">
 							<div class="header-right-content">
								<button type="button" class="boton">Login</button>
								<button type="button" class="boton">Registro</button>
 							</div>
 						</div>
 					</div>
 				</div>
 			</div>
 		</div>
 	</header>
</template>

<style scoped>
.azul {
    color: black; 
  }
  .boton{
	margin-right: 10px;
	background-color: #1e90ff;
	color: azure;
	padding: 4px;
	width: 100px;
    height: 40px;
	margin-right: 10px;
	border: 1px solid #ccc;
  }
  .imagen{
	width: 60%;
  }
</style>