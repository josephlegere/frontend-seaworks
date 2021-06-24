<template>
	<v-app dark>
		<v-navigation-drawer
			v-model="drawer"
			fixed
			app
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
		>
			<v-app-bar-nav-icon @click.stop="drawer = !drawer" />
			<v-toolbar-title v-text="title" />

			<v-spacer></v-spacer>

			<v-btn-toggle
				v-model="navigate"
				group
				:dense="$vuetify.breakpoint.smAndDown"
			>
				<v-btn value="home">Home</v-btn>
				<v-btn value="service">Service</v-btn>
				<v-btn value="about">About</v-btn>
				<v-btn value="contact">Contact</v-btn>
			</v-btn-toggle>
		</v-app-bar>
		<v-main>
			<v-container>
				<nuxt />
			</v-container>
		</v-main>
		<v-footer
			app
		>
			<span>&copy; {{ new Date().getFullYear() }}</span>
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
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      title: 'Seaworks'
    }
  }
}
</script>
