<script setup>

import { onMounted, ref} from 'vue'

import axios from "axios";

const features = ref([]);

onMounted(async () => {
  const { data: fetchedFeatures } = await axios.get("/data/features.json");
  features.value = fetchedFeatures.features;
});


</script>

<template>
     <div class="about-area section-padding">
 		<div class="container">
			<!--h1>hola</h1> --->
 			<div class="row align-items-center">
 				<div class="col-lg-6 col-md-12 col-sm-12">
					<div class="about-img-wrap">
                    <div class="image-one wow fadeInUp" data-wow-delay=".2s" style="visibility: visible; animation-delay: 0.2s; animation-name: fadeInUp;">
                        <img src="/assets/img/mano.jpg" alt="">
                    </div>                        
                    <!----div class="image-two wow fadeInUp" data-wow-delay=".4s" style="visibility: visible; animation-delay: 0.4s; animation-name: fadeInUp;">
                        <img src="/assets/img/about/about-page-2.jpg" alt="">
                    </div>  --->                                          
                </div> 					
 				</div>
 				<div class="col-lg-6 col-md-12 col-sm-12">
 					<div>
						<div class="section-title">
    <h2 class="titulo"><span class="punto"></span>Automatiza proceso de pago</h2>
</div>
 						<p> Ea enim et, similique minus soluta ipsum dolor sit, amet consectetur adipisicing elit.</p>
 						<div class="about-list-item mt-30">
							<p class="highlight">Since our launch in 1995, to deliver high value project.</p>
							<p class="highlight">We always provide flexible & quality task. </p>
							<p class="highlight">Uninque latest machinary used the industrial project.</p>
						</div>

 						<!---div class="row founded">
 							<div class="col-lg-4 col-md-6 col-12">
 								<div class="years"><span>25</span>Year of Success</div>
 							</div>
 							<div class="col-lg-8 col-md-6 col-12">
 								<div class="text">Since we established in 1995 experience &amp; still a growing protfolio day by day!</div>
 							</div>
 						</div> --->
 					</div>
 				</div>

 			</div>
 		</div>
 	</div>
</template>

<style scoped>
.imagen{
	width: 80%;
	margin: 1px;
}
.titulo {
        display: flex;
        align-items: center;
		font-size: 30px;
	margin: 1px;
    }
    .punto {
        width: 30px;
        height: 20px;
        background-color: #1e90ff;
        border-radius: 50%;
        margin-right: 10px;
    }
	.section-title h2 {
    display: inline;
}
</style>

<!---div class="feature-area section-padding">
	<div class="container">
		<div class="row">
			<div class="col-lg-6 col-md-12 col-sm-12">
				<div class="section-title">
					<h6>Features</h6>
					<h2> We manage & organized Quality <b>Industrial</b> Project</h2>
				</div>
				<div class="single-feature-item"
			   v-for="feature in features.slice(0,3)" :key="feature.id"
			   >
					<div class="feature-icon">
						<i :class="feature.icon"></i>
					</div>
					<div class="feature-content">
						<h5>{{ feature.title }}</h5>
						<p>{{ feature.content }}</p>
					</div>
				</div> 					
			</div>
			<div class="col-lg-6 col-md-12 col-sm-12">
				<div class="feature-image">
					<img src="/assets/img/feature/feature.png" alt="">
				</div>
			</div>
		</div>
	</div>
</div>---->