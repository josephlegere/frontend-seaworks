<template>
	<v-app dark>
		<v-navigation-drawer
			v-model="drawer"
			fixed
			app
			right
			:stateless="!$vuetify.breakpoint.smAndDown"
		>
			<v-list>
				<v-list-item
					v-for="(item, i) in items"
					:key="i"
					:to="item.to"
					router
					exact
				>
					<v-list-item-action>
						<v-icon>{{ item.icon }}</v-icon>
					</v-list-item-action>
					<v-list-item-content>
						<v-list-item-title v-text="item.title" />
					</v-list-item-content>
				</v-list-item>
			</v-list>
		</v-navigation-drawer>

		<v-app-bar
			fixed
			app
			dense
		>
			<v-img src="https://static.wixstatic.com/media/b69375_088b1408dc3d42a2a5e3a93f773b142a~mv2.png/v1/fill/w_362,h_103,al_c,q_85,usm_0.66_1.00_0.01/SEAWORKS%20PNG.webp" max-height="50" max-width="150" class="ml-md-6"></v-img>

			<v-spacer></v-spacer>

			<v-btn-toggle
				v-model="navigate"
				group
				:dense="$vuetify.breakpoint.smAndDown"
				class="d-none d-md-block"
			>
				<v-btn
					v-for="(item, i) in items"
					:key="i"
					:value="item.title"
					@click="$vuetify.goTo(item.to)"
				>{{ item.title }}</v-btn>
			</v-btn-toggle>

			<v-app-bar-nav-icon @click.stop="drawer = !drawer" class="d-md-none" />
		</v-app-bar>
		<v-main>
			<nuxt />
		</v-main>
		<v-footer
			app
		>
			<span>Seaworks Coompany. &copy; {{ new Date().getFullYear() }}</span>
		</v-footer>
	</v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: false,
	  navigate: 'home',
      items: [
        {
          icon: 'mdi-apps',
          title: 'Home',
          to: '#home'
        },
        {
          icon: 'mdi-toolbox-outline',
          title: 'Service',
          to: '#service'
        },
        {
          icon: 'mdi-information-outline',
          title: 'About',
          to: '#about'
        },
        {
          icon: 'mdi-account-box-outline',
          title: 'Contact',
          to: '#contact'
        }
      ],
      title: 'Seaworks'
    }
  }
}
</script>
