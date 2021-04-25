<template>
<div>
 <h1>OFFRES DE STAGES DISPONIBLES</h1>
<section class="buckets grid" id="bucketsgrid">
    <ul>
       <li  v-for="item in shoppingCart" v-bind:key="shoppingCart.indexOf(item)" >
        <img src="../assets/bulding.svg" alt="">
        <div class="bucket">
          <h3 class="bucket-title"> {{ item.label }}</h3>
          <p> {{ item.entreprise }} </p>
	<router-link :to="{path:item.url}">
	<b-button variant="warning">DÉTAILS</b-button>
		</router-link>
        <router-view/>
        </div>
      </li>
    </ul>
</section>
</div>
</template>
<script>

export default {
        data ()
         {
           return {
             shoppingCart: [
                { label: 'développeur web junior', entreprise: 'Sodson Corp', img_path: "../assets/Epitech.png", url:"/aboutjob" },
                { label: 'Assistant pédagogique', entreprise: 'Epitech bénin', img_path: "../assets/Epitech.png", url:"/aboutjob1" },
                { label: 'Technicien réseau junior', entreprise: 'Bénin Télécom', img_path: "../assets/Epitech.png", url:"/aboutjob2" }
            ]
           }
           }
    }

</script>

<style>

/*--------------------------------------------------------------
CSS Reset
--------------------------------------------------------------*/

/*#bucketsgrid {
	display:flex;
}*/


#bucketsgrid img {
	display: block;
	border: 0;
	width: 100%;
	height: auto;
}

/*--------------------------------------------------------------
Typography
--------------------------------------------------------------*/
body,
button,
input,
select,
textarea {
	color: #404040;
	font-family: 'Helvetica', Arial, sans-serif;
	font-size: 18px;
	line-height: 1.5;
}

h1,
h2,
h3 {
	text-align: center;
	margin: 0;
	padding: 1em 0;
}

p {
	margin: 0;
	padding: 1em 0;
}

/* Buckets section */

.buckets {
	padding: 2em 1em 1em;
	background: #3E454C;
}

.buckets ul {
	margin: 0;
	padding: 0;
}

.buckets li {
	margin-bottom: 1em;
	background: white;
	list-style-type: none;
}

.bucket {
	padding: 1.5em;
}

/* More section */

.more {
	padding: 2em;
}

/*--------------------------------------------------------------
If no grid support, limit width to 50em and center align
--------------------------------------------------------------*/
@supports not (display: grid) {
	.grid {
		max-width: 50em;
		margin: 0 auto;
	}
}

/*--------------------------------------------------------------
Use flex to create a three-bucket layout 
--------------------------------------------------------------*/

@media screen and (min-width: 700px) {
	@supports (display: flex) {

		.buckets ul {
			display: flex;
			justify-content: space-around;
		}

		.buckets li {
			width: 31%;
		}

	}
}

/*--------------------------------------------------------------
CSS Grid layout for wider screens, when browser supports grid:
--------------------------------------------------------------*/

@media screen and (min-width: 600px) {
	/* Layout with CSS Grid */
	@supports (display: grid) {

		/* Four-column layout. Two center columns have a total max width of 50em: */
		.grid {

			display: grid;
			grid-template-columns: 1fr repeat(2, minmax(auto, 25em)) 1fr;
		}

		/* Center items by placing them in the two center columns: */
		.splash-content,
		.more-content,
		.buckets ul {
			grid-column: 2/4;
		}

	}
}

</style>