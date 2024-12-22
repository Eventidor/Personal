		<template>
	<div class="contact-form">
		<h2> Contact Me </h2>
		<form @submit.prevent="submitForm">
			<div class="form-group">
				<label for="name">Name: </label>
				<input type="text" id="name"v-model="form.name"required/>
			</div>
			<div class="form-group">
				<label for="email">Email: </label>
				<input type="email"id="email" v-model="form.email" required/>
			</div>
			<div class="form-group">
				<label for="message">Message: </label>
				<textarea id="message" v-model="form.message"required></textarea>
			</div>
			<button type="submit">Send Message</button>
		</form>
		<p v-if="statusMessage":class="statusClass"> {{ statusMessage }}</p>
	</div>
</template>
<script>
export default {
	data(){
		return{
		form: {
			name:  '',
			email: '',
			message: ''
		},
		statusMessage: '',
		statusClass: '',
	};
},
	methods: {
		submitForm(){
			this.statusMessage ='Thank you for Messaging';
			this.statusClass='success';
			this.form.name='';
			this.form.email='';
			this.form.message='';
		},
	},
};

</script>
<style scoped>
.contact-form{
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	height: 100vh;
	text-align: center;
}
.form-group{
	margin-bottom: 15px;
}
form{
	width: 100%;
	max-width: 400px;
	padding: 20px;
	border: 1px solid #ccc;
	background-color: white;
	border-radius: 8px;
}
button{
	background-color: green;
	color: white;
	padding: 10px 20px;
	border: none;
	cursor: pointer;
	width: 100%;
	font-size: 16px;
	margin-top: 10px;
	border-radius: 4px;
}
label{
	color: black;
}
button:hover{
	background-color: #34ff;
}
.success{
	color: green;
	font-weight: bold;
	margin-top: 20px;
}
</style>
