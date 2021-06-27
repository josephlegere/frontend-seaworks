<template>
	<v-row no-gutters align="center">
		<v-col cols="12" id="home">
			<v-card :height="$vuetify.breakpoint.smAndDown?'auto':'90vh'">
				<video autoplay muted loop id="myVideo" width="100%">
					<source src="https://video.wixstatic.com/video/b69375_74e256e6b7cf42f29b9b6fe396b7689d/1080p/mp4/file.mp4" type="video/mp4">
				</video>
				<div class="custom-card-title text-right text-h6 text-md-h3 mb-md-6">
					<strong>TRUSTED PARTNER<br>IN MARINE CONSTRUCTIONS</strong>
				</div>
				<div class="custom-card-text">
					<v-list style="background: transparent;" :dense="$vuetify.breakpoint.smAndDown" class="ml-md-6">
						<v-list-item class="my-md-2" v-for="(item, i) in featured" :key="i">
							<v-list-item-content class="cyan--text text--lighten-5 text-md-h6">{{item}}</v-list-item-content>
						</v-list-item>
					</v-list>
				</div>
				<!-- <v-img
					src="https://video.wixstatic.com/video/b69375_74e256e6b7cf42f29b9b6fe396b7689d/1080p/mp4/file.mp4"
					height="100%"
					class="grey darken-4"
				></v-img> -->
			</v-card>
		</v-col>

		<v-col cols="12" id="service">
			<v-card class="text-center" tile>
				<div class="text-h6 text-md-h4 font-weight-medium custom-header py-3">Our Services</div>
			</v-card>
			<v-row no-gutters>
				<v-col cols="12" md="6" v-for="(service, i) in services" :key="i">
					<v-card class="text-center" tile min-height="320">
						<v-img :src="service.image" width="200" class="mx-auto"></v-img>
						<v-card-title class="justify-center">{{service.title}}</v-card-title>
						<v-card-text class="text-justify">{{service.description}}</v-card-text>
					</v-card>
				</v-col>
			</v-row>
		</v-col>

		<v-col cols="12">
			<v-parallax src="http://localhost:3000/blue-bg.jpg" height="200"></v-parallax>
		</v-col>

		<v-col cols="12" id="about">
			<v-card>
				<v-row no-gutters>
					<v-col cols="12" md="6">
						<v-card-title>Our Story</v-card-title>
						<v-card-text class="text-justify">
							Seaworks Co was founded in Kuwait in 1991 as Mubarakia Marine Service Co., as a marine services contractor. We have expanded our activities to include Marine Construction, Ship Management, Heavy Equipment Rentals, and Earthworks.
​
							With the technology transfer scheme that the government of Kuwait had opted for; we initiated a long-term business plan to develop strong alliances with international companies for streamlining future projects in Kuwait. Our most notable relationship was established in 1996, with ITOCHU Corporation, a Japanese trading house, and this relationship developed into a very close strategic alliance for mutual business interests in Kuwait. This was further enhanced by establishing a long-term association with Tekfen Construction & Installation Company, and an agency agreement was signed in 2005 with Tekfen in Kuwait.

							Our parent company, Khalil Mahmoud Trading & Contracting Est. (KME) was established in 1953, primarily as a civil engineering and construction company, and has been classified as a Grade II contractor by the Central Tenders Committee since 1971 for civil construction and electrical works, which is the highest category given to local contractors working in Kuwait as category I is for international contractors. KME is best known for developing the State of Kuwait’s tenth district (Cities of Fahaheel, Ahmadi, Sabahiya, Mangaf, AbuHalifa, Fintas) by the construction of housing & commercial projects as well as relevant municipal infrastructure. In addition, KME pioneered the development of farming and mass agricultural production in Kuwait by implementing horticultural farming in the Wafra area.
						</v-card-text>
					</v-col>
					<v-col cols="12" md="6">
						<v-img src="https://static.wixstatic.com/media/b69375_f7cfe407cc774592a88f28b62b12362b~mv2.jpg/v1/fill/w_630,h_420,al_c,lg_1,q_80/bg%20copy.webp" height="100%"></v-img>
					</v-col>
				</v-row>
			</v-card>
		</v-col>

		<v-col cols="12" md="6" class="my-6" offset-md="3" id="contact">
			<v-card flat tile>
				<v-card-title class="headline">
					Contact Us
				</v-card-title>
				<v-card-text>
					<v-row no-gutters>
						<v-col cols="12">
							<v-text-field
								label="Name"
							></v-text-field>
						</v-col>
						<v-col cols="12">
							<v-text-field
								label="Email"
							></v-text-field>
						</v-col>
						<v-col cols="12">
							<v-text-field
								label="Phone"
							></v-text-field>
						</v-col>
						<v-col cols="12">
							<v-textarea
								label="Message"
								autoGrow
								dense
								hide-details
								rows="3"
							></v-textarea>
						</v-col>
					</v-row>
				</v-card-text>
				<v-card-actions>
					<v-spacer />
					<v-btn
						color="primary"
						nuxt
						to="/inspire"
					>
						Submit
					</v-btn>
				</v-card-actions>
			</v-card>
		</v-col>

		<v-col cols="12" md="6" class="my-6 px-2" offset-md="3">
			<v-card flat tile>
					<v-row no-gutters>
						<v-col cols="12">
							<v-list>
								<v-list-item-title class="text-h5">Working Hours</v-list-item-title>
								<v-list-item-content>
									<v-row
										align="center"
										justify="start"
										class="mt-1"
									>
										<v-icon class="ml-3 mr-1">
											mdi-calendar
										</v-icon>
										<span class="subheading">Sunday - Thursday, 7:00 AM - 5:00 PM</span>
									</v-row>
								</v-list-item-content>
							</v-list>
						</v-col>
						<v-col cols="12">
							<v-list>
								<v-list-item-title class="text-h5">Contact Us</v-list-item-title>
								<v-list-item-content>
									Your feedback is important to Seaworks. Share with us your comments, compliments and feedback to help us improve our services.
								</v-list-item-content>

								<v-list-item-content>
									<v-row
										align="center"
										justify="start"
										class="mt-1"
									>
										<v-icon class="ml-3 mr-1">
											mdi-map-marker
										</v-icon>
										<span class="subheading">Seaworks Co, Building No 36, Street No 913,<br> Next to Spanish Embassy, P.O Box 23631.</span>
									</v-row>
								</v-list-item-content>
								<v-list-item-content>
									<v-row
										align="center"
										justify="start"
										class="mt-1"
									>
										<v-icon class="ml-3 mr-1">
											mdi-phone
										</v-icon>
										<span class="subheading">Tel: (+974) 4411 0455</span>
									</v-row>
								</v-list-item-content>
								<v-list-item-content>
									<v-row
										align="center"
										justify="start"
										class="mt-1"
									>
										<v-icon class="ml-3 mr-1">
											mdi-fax
										</v-icon>
										<span class="subheading">Fax: (+974) 4411 0921</span>
									</v-row>
								</v-list-item-content>
								<v-list-item-content>
									<v-row
										align="center"
										justify="start"
										class="mt-1"
									>
										<v-icon class="ml-3 mr-1">
											mdi-email
										</v-icon>
										<span class="subheading">info@seaworks.net</span>
									</v-row>
								</v-list-item-content>
								<v-list-item-content><v-row
										align="center"
										justify="start"
										class="mt-1"
									>
										<v-icon class="ml-3 mr-1">
											mdi-web
										</v-icon>
										<span class="subheading">www.seaworks.net</span>
									</v-row>
								</v-list-item-content>
							</v-list>
						</v-col>
					</v-row>
			</v-card>
		</v-col>
	</v-row>
</template>

<script>

export default {
	data () {
		return {
			featured: [
				'Marine Construction',
				'Ship Management',
				'Heavy Equipment Rental',
				'Earth Works',
				'Rental'
			],
			services: [
				{
					title: 'Marine Construction',
					description: 'Seaworks is a leading marine civil engineering firm and renowned foreshore specialist in Kuwait and Qatar. Our services range from revetment, seawall, breakwater, rock bund construction...',
					image: 'https://static.wixstatic.com/media/b69375_ce30945edfaa4e35b77d6b1e1c35b505~mv2.png/v1/fill/w_560,h_414,al_c,lg_1,q_85/icon-startsite-dredger.webp'
				},
				{
					title: 'SHIP MANAGEMENT',
					description: 'Seaworks is an independent marine-services provider offering a broad scope of high quality ship management and consultancy services for all types of vessels and offshore units..',
					image: 'https://static.wixstatic.com/media/b69375_c2e9c0580ee44ab8a2de9492389f4270~mv2.png/v1/fill/w_346,h_214,al_c,q_85,usm_0.66_1.00_0.01/clipart-boat-icon-3.webp'
				},
				{
					title: 'HEAVY EQUIPMENT RENTAL',
					description: 'Our steady growth and expansion has transformed the company to be one of the major marine construction companies. This has led to a policy of investment in equipment and an expansion...',
					image: 'https://static.wixstatic.com/media/b69375_6bcf047258dd47218e1274a1205ab021~mv2.png/v1/fill/w_250,h_214,al_c,q_85,usm_0.66_1.00_0.01/14-148424_crane-svg-png-icon-free-downlo.webp'
				},
				{
					title: 'EARTHWORKS',
					description: 'With our extensive service experience of more than 22years in the Marine Industry, combined with the ability to handle the local market demand, providing engineering solutions that make us a reliable partner...',
					image: 'https://static.wixstatic.com/media/b69375_8c95ea55e9724db384871bb26e04bcfd~mv2.png/v1/fill/w_370,h_214,al_c,q_85,usm_0.66_1.00_0.01/img_455142.webp'
				}
			]
		}
	}
}
</script>

<style scoped>
	.custom-card-title {
		position:					absolute;
		bottom:						0;
		color:						aliceblue;
		width:						100%;
		padding:					20px;
		font-family:				'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
	}
	.custom-card-text {
		position:					absolute;
		top:						5%;
		left:						0;
		color:						aliceblue;
		font-family:				'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
	}
	.custom-header {
		font-family:				'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif !important;
	}
</style>