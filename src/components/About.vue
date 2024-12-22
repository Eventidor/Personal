<template>
	<section class="about">
		<div class="container">
			<h1> About Me </h1>
			<p class="intro">
				Hi, I'm <strong> Farhan Khatri</strong>, a self-taught Programmer and a Computer Engineering Diploma Student at <strong>Parul Polytechnic Institute</strong>. I'm passionate about developing innovative solutions and continuously learning new technologies. My journey as a programmer began out of curiosity, and over the years, I've developed a love for coding and problem-solving. 
			</p>
			<div class="about-content">
			<div class="bio">
			<h2>My Journey</h2>
			<p>
			I Started My Programming Journey by exploring various online resources and tutorials. As a self-taught programmer, I learned through hands-on practice and real-world projects. While studying computer engineering, I have been able to complement my formal education with practical coding experience, allowing me to grow as a developer.
			</p>
			<p>
			I belive that learning never stops, and my goal is to continue honing my skills in full-stack web development and contribute to the tech community. Though I am still a student, I'm dedicated to building meaningful projects that solve real world problems. 
			</p>
			</div>
			<div class="skill">
				<ul>
					<li>Frontend Development: Html ,CSS ,Javascript ,PHP </li>
					<li>Backend Development: Node.js ,Express </li>
					<li>Version Control: Git ,Github </li>
					<li>Database: MongoDB ,MySQL </li>
					<li>Problem Solving &amp; Algorithms</li>
				</ul>
			</div>
			<div class="current-project">
				<h2>Current Project</h2>
				<p>
				I am currently working on improving my portfolio and building full-stack applications that demonstrate my ability to create functional and efficient systems. I am also exploring new technologies and opportunities to collaborate with other developers and contribute to open-source projects.
				</p>
			</div>
		 </div>
		</div>
		<a href="https://www.github.com/Eventidor"target="_blank"><img src="./logo/github-logo.png" height="55px"width="55px"alt="Github Logo"/></a>
		<a href="https://www.instagram.com/farhan_khatri65"target="_blank"><img src="https://1000logos.net/wp-content/uploads/2017/02/Instagram-Logo-2010-2013.png" height="55px"width="55px"></a>
	</section>
</template>
<script>
	export default {
		name: "About",
	};
</script>
<style scoped>
.about{
	padding: 50px 0;
	background-color: #f9f9f9;
	font-family: Arial, sans-serif;
}
.container {
	width: 80%;
	margin: 0 auto;
}
h1{
	font-size: 36px;
	color: #333;
	text-align: center;
	margin-bottom: 20px;
}
.intro{
	font-size: 18px;
	color: #333;
	text-align: center;
	margin-bottom: 40px;
}
.about-content{
	display: flex;
	justify-content: space-between;
	gap: 40px;
}
.bio,
.skill,
.current-project{
	width: 30%;
}
.bio h2,
.skills h2, 
.current-project h2,p{
	font-size: 24px; 
	color: #333; 
	margin-bottom: 10px; 
} 
ul { 
	list-style-type: none; 
	padding-left: 0; 
} 
ul li{ 
	font-size: 16px; 
	color: #555; 
	margin-bottom: 5px; 
	font-weight: strong;
} 
@media (max-width: 768px) { 
	.about-content { 
		flex-direction: column; 
		align-items: center; 
	} 
	
	.bio,
	.skill, 
	.current-project { 
		width: 80%; 
		margin-bottom: 20px; 
	} 
}
a{
	margin: 20px;
}
</style>
