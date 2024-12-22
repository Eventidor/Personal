<template>
	<h1>Farhan Khatri's Portfolio</h1>
	<button class="btn primay-btn"@click="this.showAbout = !this.showAbout">About</button>
	<br /><br />
	<About v-if="showAbout" />
	<button class="btn primary-btn" @click="this.showContact = !this.showContact">Contact</button>
	<Contact v-if="showContact" />
</template>
<script>
	import About from './About.vue'
	import Contact from './Contact.vue'
	export default{
		components: {
			About,
			Contact,
		},data() {
			return{
				showAbout: false,
				showContact: false,
			};
		},
	};
</script>
<style>
button{
	background-color: #00f;
}
button:hover{
	background-color: #5f5;
	border-color: 30px solid red;
}
</style>
