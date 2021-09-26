<script>
	import Content from './content.svelte';
</script>

<main>
	<header class="shadow">
		<h1> Rose Villaluna </h1>
		<p> “For God so loved the world that he sent His only begotten son to save the people and would have eternal life with Him.” </p>
		<img class="avatar shadow" src="https://scontent.fmnl17-3.fna.fbcdn.net/v/t1.6435-9/241967965_3046291718993914_7971090436232087753_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=09cbfe&_nc_eui2=AeFz8IE-EHu8zkHF6LPpdid5JiOvCmW8LRgmI68KZbwtGHmenBfbUQJZYa294Fap_5eyy9iAxIl4uu13ha8jDAOq&_nc_ohc=RyvjIGtK358AX9pqELA&_nc_ht=scontent.fmnl17-3.fna&oh=d987f887eed645d801d673037b441b99&oe=6176E1A1" alt="Rose Villaluna" />
	</header>
	<section class="outlined rounded">
		<nav>
			<a href="#about-me"> About Me </a>
			<a href="#about-my-course"> About My Course </a>
			<a href="#reflection"> Reflection On The Course </a>
			<a href="#dream"> My Dream </a>
			<a href="#prof"> Professor </a>
		</nav>
	</section>

	<section class="outlined rounded" id="landing">
		<div>
			<h1> Hi, I am Rose Anne Villaluna. Thank you for visiting my e-portfolio. </h1>
			<br>
			<p> Taking Bachelor of Science in Secondary Education Major in Social Studies in Pamantasan ng Lungsod ng Muntinlupa. </p>
		</div>
		<!-- svelte-ignore a11y-media-has-caption -->
		<video class="shadow rounded" src="rose.mp4" autoplay controls></video>
	</section>

	<section class="outlined rounded note">
		<p>
			As I did my Digital Media Output I was very amazed and astonished at how the technology help me to boost my confidence and widen my understanding of media.  At first it was hard to use and explore some apps that am gonna use, but at the end, I do love learning how to do and make an amazing output. Guess what? I got 92% of Grades🤗. It's not a high score for everyone, but I take it as a lesson to remind myself to improve. 
		</p>
	</section>

	<Content/>

	<section class="outlined rounded">
		<nav>
			<a href="https://www.facebook.com/roseanne.villaluna.9"> Facebook </a>
			<a href="https://www.instagram.com/roserosevillaluna"> Instagram </a>
		</nav>
	</section>
	<br>
</main>

	<style>
	@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');

	header p {
		color: white;
		font-family: 'Lobster', cursive;
		font-weight: 100;
		text-align: center;
		padding: 1rem;
	}

	#landing {
		display: flex;
		gap: 2rem;
		padding: 2rem;
	}

	#landing h1 {
		font-size: 3rem;
		background: linear-gradient(90deg,#ff0077, #c300ff, dodgerblue, #ff0077);
		background-clip: text;
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}

	#landing video {
		width: 50%;
	}

	nav {
		display: flex;
		gap: 1rem;
	}
	header {
		width: 100%;
		height: 40vh;
		background: linear-gradient(90deg,#ff0077, #c300ff, dodgerblue, #ff0077);
		background-size: 300%;
		background-position: 0;
		position: relative;
		animation: shine 20s infinite;
		margin-bottom: 7rem;
		border-bottom: .25rem solid white;
	}
	header h1 {
		color: white;
		font-family: 'Lobster', cursive;
		font-weight: 400;
		text-align: center;
		padding: 1rem 0 0 0;
		font-size: 5rem;
	}
	header .avatar {
		display: block;
		position: relative;
		width: 10rem;
		height: 10rem;
		border-radius: 50%;
		border: .25rem solid white;
		margin: auto;
	}
	section {
		margin: 1rem;
		padding: 1rem;
		background-color: var(--surface1);
	}
	@media (max-width: 650px) {
		nav {
			flex-direction: column;
		}
	}
	@media (max-width: 560px) {
		header h1 {
			font-size: 3rem;
			top: 1rem;
		}
		header {
			height: 30vh;
		}
		nav {
			flex-direction: column;
		}
		#landing {
			flex-direction: column;
			padding: 1rem;
		}
		#landing h1 {
			font-size: 1.5rem;
		}
		#landing h1, #landing p {
			text-align: center;
		}
		#landing video {
			width: 100%;
		}
	}
</style>