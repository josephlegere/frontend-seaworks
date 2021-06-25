<template>
	<v-row no-gutters justify="center" align="center">
		<v-col cols="12">
			<v-card>
				<video autoplay muted loop id="myVideo" width="100%" height="100%">
					<source src="https://video.wixstatic.com/video/b69375_74e256e6b7cf42f29b9b6fe396b7689d/1080p/mp4/file.mp4" type="video/mp4">
				</video>
				<div class="custom-card-title text-right">
					<h1>TRUSTED PARTNER IN MARINE CONSTRUCTIONS</h1>
				</div>
				<!-- <v-img
					src="https://video.wixstatic.com/video/b69375_74e256e6b7cf42f29b9b6fe396b7689d/1080p/mp4/file.mp4"
					height="100%"
					class="grey darken-4"
				></v-img> -->
			</v-card>
		</v-col>

		<v-col cols="12">
			<v-row no-gutters>
				<v-col cols="6">
					<v-card>
						<v-avatar>
							<v-img src="https://static.wixstatic.com/media/b69375_ce30945edfaa4e35b77d6b1e1c35b505~mv2.png/v1/fill/w_560,h_414,al_c,lg_1,q_85/icon-startsite-dredger.webp"></v-img>
						</v-avatar>
						<v-card-title>Marine Construction</v-card-title>
						<v-card-text>
							Seaworks is a leading marine civil engineering firm and renowned foreshore specialist in Kuwait and Qatar. Our services range from revetment, seawall, breakwater, rock bund construction...
						</v-card-text>
					</v-card>
				</v-col>
				<v-col cols="6">
					<v-card>
						<v-avatar>
							<v-img src="https://static.wixstatic.com/media/b69375_ce30945edfaa4e35b77d6b1e1c35b505~mv2.png/v1/fill/w_560,h_414,al_c,lg_1,q_85/icon-startsite-dredger.webp"></v-img>
						</v-avatar>
						<v-card-title>SHIP MANAGEMENT</v-card-title>
						<v-card-text>
							Seaworks is an independent marine-services provider offering a broad scope of high quality ship management and consultancy services for all types of vessels and offshore units..
						</v-card-text>
					</v-card>
				</v-col>
			</v-row>
		</v-col>

		<v-col cols="12">
			<v-card>
				<v-row no-gutters>
					<v-col cols="12" md="6">
						<v-card-title>Our Story</v-card-title>
						<v-card-text>
							Seaworks Co was founded in Kuwait in 1991 as Mubarakia Marine Service Co., as a marine services contractor. We have expanded our activities to include Marine Construction, Ship Management, Heavy Equipment Rentals, and Earthworks.
​
							With the technology transfer scheme that the government of Kuwait had opted for; we initiated a long-term business plan to develop strong alliances with international companies for streamlining future projects in Kuwait. Our most notable relationship was established in 1996, with ITOCHU Corporation, a Japanese trading house, and this relationship developed into a very close strategic alliance for mutual business interests in Kuwait. This was further enhanced by establishing a long-term association with Tekfen Construction & Installation Company, and an agency agreement was signed in 2005 with Tekfen in Kuwait.

							Our parent company, Khalil Mahmoud Trading & Contracting Est. (KME) was established in 1953, primarily as a civil engineering and construction company, and has been classified as a Grade II contractor by the Central Tenders Committee since 1971 for civil construction and electrical works, which is the highest category given to local contractors working in Kuwait as category I is for international contractors. KME is best known for developing the State of Kuwait’s tenth district (Cities of Fahaheel, Ahmadi, Sabahiya, Mangaf, AbuHalifa, Fintas) by the construction of housing & commercial projects as well as relevant municipal infrastructure. In addition, KME pioneered the development of farming and mass agricultural production in Kuwait by implementing horticultural farming in the Wafra area.
						</v-card-text>
					</v-col>
					<v-col cols="12" md="6">
						<v-img src="https://static.wixstatic.com/media/b69375_f7cfe407cc774592a88f28b62b12362b~mv2.jpg/v1/fill/w_630,h_420,al_c,lg_1,q_80/bg%20copy.webp"></v-img>
					</v-col>
				</v-row>
			</v-card>
		</v-col>

		<v-col cols="12">
			<v-card>
				<v-card-title class="headline">
					Welcome to the Vuetify + Nuxt.js template
				</v-card-title>
				<v-card-text>
					<p>Vuetify is a progressive Material Design component framework for Vue.js. It was designed to empower developers to create amazing applications.</p>
					<p>
						For more information on Vuetify, check out the
							<a
							href="https://vuetifyjs.com"
							target="_blank"
							rel="noopener noreferrer"
						>
							documentation
						</a>.
					</p>
					<p>
						If you have questions, please join the official
						<a
							href="https://chat.vuetifyjs.com/"
							target="_blank"
							rel="noopener noreferrer"
							title="chat"
						>
							discord
						</a>.
					</p>
					<p>
						Find a bug? Report it on the github
						<a
							href="https://github.com/vuetifyjs/vuetify/issues"
							target="_blank"
							rel="noopener noreferrer"
							title="contribute"
						>
							issue board
						</a>.
					</p>
					<p>Thank you for developing with Vuetify and I look forward to bringing more exciting features in the future.</p>
					<div class="text-xs-right">
						<em><small>&mdash; John Leider</small></em>
					</div>
				</v-card-text>
				<v-card-actions>
					<v-spacer />
					<v-btn
						color="primary"
						nuxt
						to="/inspire"
					>
						Continue
					</v-btn>
				</v-card-actions>
			</v-card>
		</v-col>
	</v-row>
</template>

<script>


export default {
}
</script>

<style scoped>
	.custom-card-title {
		position:					absolute;
		bottom:						0;
		color:						aliceblue;
		width:						100%;
		padding:					20px;
		font-family:				'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif
	}
</style>