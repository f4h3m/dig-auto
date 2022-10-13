<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/logo.svg';
	import black_logo from '$lib/images/black-logo.svg';
	import side_image from '$lib/images/socialbar_bg.png';

	import menu_icon from '$lib/images/menu-icon.svg';
	import ico_close2 from '$lib/images/ico-close2.svg';

	let height;
	let hide_bar = false;
	let open = false;
	let endOpen = false;
	const toggleEnd = () => (endOpen = !endOpen);
</script>

<svelte:window bind:scrollY={height} />

<header class:sticky-nav={height > 50}>
	<div class="container">
		<div class="row align-items-center justify-content-end">
			{#if $page.url.pathname === '/' || $page.url.pathname === '/careers'}
				<div class="col-4">
					{#if height > 50}
						<a href="/"><img src={black_logo} alt="" /></a>
					{/if}
					{#if height < 50}
						<a href="/"><img src={logo} alt="" /></a>
					{/if}
				</div>
				<div class="col-8">
					<ul class="d-flex justify-content-end main-menu normal-state">
						<li><a href="/">Home</a></li>
						<li><a href="/company">Company</a></li>
						<li><a href="/team">Team</a></li>
						<li><a href="/news">News</a></li>
						<li><a href="/careers">Careers</a></li>
						<li><a href="https://cloudcastles.gg/">Games</a></li>
					</ul>
					<span class="menu-icon" on:click={() => (endOpen = !endOpen)}>
						<img src={menu_icon} alt="" />
					</span>
				</div>
			{:else}
				<div class="col-4">
					{#if height > 50}
						<a href="/"><img src={black_logo} alt="" /></a>
					{/if}
					{#if height < 50}
						<a href="/"><img src={black_logo} alt="" /></a>
					{/if}
				</div>
				<div class="col-8">
					<ul class="d-flex justify-content-end main-menu">
						<li><a href="/">Home</a></li>
						<li><a href="/company">Company</a></li>
						<li><a href="/team">Team</a></li>
						<li><a href="/news">News</a></li>
						<li><a href="/careers">Careers</a></li>
						<li><a href="https://cloudcastles.gg/">Games</a></li>
					</ul>
					<span class="menu-icon" on:click={() => (endOpen = !endOpen)}>
						<img src={menu_icon} alt="" />
					</span>
				</div>
			{/if}
		</div>
	</div>
</header>

<div class="side_social" class:hide_bar>
	<span class="social_close">✖</span>
	<span on:click={() => (hide_bar = !hide_bar)} class="social_on_off" />
	<ul style="background-image: url({side_image});">
		<li>
			<a
				href="https://discord.gg/DIG"
				target="_blank"
				class="sns-discord"
				title="Open The Discord Link In A New Window"
			>
				<!--?xml version="1.0" encoding="UTF-8"?-->
				<svg
					width="256px"
					height="256px"
					viewBox="0 -28.5 256 256"
					version="1.1"
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					preserveAspectRatio="xMidYMid"
				>
					<g>
						<path
							d="M216.856339,16.5966031 C200.285002,8.84328665 182.566144,3.2084988 164.041564,0 C161.766523,4.11318106 159.108624,9.64549908 157.276099,14.0464379 C137.583995,11.0849896 118.072967,11.0849896 98.7430163,14.0464379 C96.9108417,9.64549908 94.1925838,4.11318106 91.8971895,0 C73.3526068,3.2084988 55.6133949,8.86399117 39.0420583,16.6376612 C5.61752293,67.146514 -3.4433191,116.400813 1.08711069,164.955721 C23.2560196,181.510915 44.7403634,191.567697 65.8621325,198.148576 C71.0772151,190.971126 75.7283628,183.341335 79.7352139,175.300261 C72.104019,172.400575 64.7949724,168.822202 57.8887866,164.667963 C59.7209612,163.310589 61.5131304,161.891452 63.2445898,160.431257 C105.36741,180.133187 151.134928,180.133187 192.754523,160.431257 C194.506336,161.891452 196.298154,163.310589 198.110326,164.667963 C191.183787,168.842556 183.854737,172.420929 176.223542,175.320965 C180.230393,183.341335 184.861538,190.991831 190.096624,198.16893 C211.238746,191.588051 232.743023,181.531619 254.911949,164.955721 C260.227747,108.668201 245.831087,59.8662432 216.856339,16.5966031 Z M85.4738752,135.09489 C72.8290281,135.09489 62.4592217,123.290155 62.4592217,108.914901 C62.4592217,94.5396472 72.607595,82.7145587 85.4738752,82.7145587 C98.3405064,82.7145587 108.709962,94.5189427 108.488529,108.914901 C108.508531,123.290155 98.3405064,135.09489 85.4738752,135.09489 Z M170.525237,135.09489 C157.88039,135.09489 147.510584,123.290155 147.510584,108.914901 C147.510584,94.5396472 157.658606,82.7145587 170.525237,82.7145587 C183.391518,82.7145587 193.761324,94.5189427 193.539891,108.914901 C193.539891,123.290155 183.391518,135.09489 170.525237,135.09489 Z"
							fill="#8d8d8d"
							fill-rule="nonzero"
						/>
					</g>
				</svg></a
			>
		</li>
		<li>
			<a
				href="https://twitter.com/DIGames__DIG"
				target="_blank"
				class="sns-twitter"
				title="Open The Twitter Link In A New Window"
			>
				<!--?xml version="1.0" encoding="iso-8859-1"?-->
				<!-- Generator: Adobe Illustrator 19.0.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
				<svg
					version="1.1"
					id="Layer_1"
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					x="0px"
					y="0px"
					viewBox="0 0 310 310"
					style="enable-background:new 0 0 310 310;"
					xml:space="preserve"
				>
					<g id="XMLID_826_">
						<path
							id="XMLID_827_"
							d="M302.973,57.388c-4.87,2.16-9.877,3.983-14.993,5.463c6.057-6.85,10.675-14.91,13.494-23.73
	   c0.632-1.977-0.023-4.141-1.648-5.434c-1.623-1.294-3.878-1.449-5.665-0.39c-10.865,6.444-22.587,11.075-34.878,13.783
	   c-12.381-12.098-29.197-18.983-46.581-18.983c-36.695,0-66.549,29.853-66.549,66.547c0,2.89,0.183,5.764,0.545,8.598
	   C101.163,99.244,58.83,76.863,29.76,41.204c-1.036-1.271-2.632-1.956-4.266-1.825c-1.635,0.128-3.104,1.05-3.93,2.467
	   c-5.896,10.117-9.013,21.688-9.013,33.461c0,16.035,5.725,31.249,15.838,43.137c-3.075-1.065-6.059-2.396-8.907-3.977
	   c-1.529-0.851-3.395-0.838-4.914,0.033c-1.52,0.871-2.473,2.473-2.513,4.224c-0.007,0.295-0.007,0.59-0.007,0.889
	   c0,23.935,12.882,45.484,32.577,57.229c-1.692-0.169-3.383-0.414-5.063-0.735c-1.732-0.331-3.513,0.276-4.681,1.597
	   c-1.17,1.32-1.557,3.16-1.018,4.84c7.29,22.76,26.059,39.501,48.749,44.605c-18.819,11.787-40.34,17.961-62.932,17.961
	   c-4.714,0-9.455-0.277-14.095-0.826c-2.305-0.274-4.509,1.087-5.294,3.279c-0.785,2.193,0.047,4.638,2.008,5.895
	   c29.023,18.609,62.582,28.445,97.047,28.445c67.754,0,110.139-31.95,133.764-58.753c29.46-33.421,46.356-77.658,46.356-121.367
	   c0-1.826-0.028-3.67-0.084-5.508c11.623-8.757,21.63-19.355,29.773-31.536c1.237-1.85,1.103-4.295-0.33-5.998
	   C307.394,57.037,305.009,56.486,302.973,57.388z"
							fill="#8d8d8d"
						/>
					</g>
				</svg></a
			>
		</li>
		<li>
			<a
				href="https://telegram.me/DigitalInsightGames"
				target="_blank"
				class="sns-telegram"
				title="Open The Telegram Link In A New Window"
			>
				<!--?xml version="1.0" encoding="iso-8859-1"?-->
				<!-- Generator: Adobe Illustrator 19.0.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
				<svg
					version="1.1"
					id="Layer_1"
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					x="0px"
					y="0px"
					viewBox="0 0 300 300"
					style="enable-background:new 0 0 300 300;"
					xml:space="preserve"
				>
					<g id="XMLID_496_">
						<path
							id="XMLID_497_"
							d="M5.299,144.645l69.126,25.8l26.756,86.047c1.712,5.511,8.451,7.548,12.924,3.891l38.532-31.412
	   c4.039-3.291,9.792-3.455,14.013-0.391l69.498,50.457c4.785,3.478,11.564,0.856,12.764-4.926L299.823,29.22
	   c1.31-6.316-4.896-11.585-10.91-9.259L5.218,129.402C-1.783,132.102-1.722,142.014,5.299,144.645z M96.869,156.711l135.098-83.207
	   c2.428-1.491,4.926,1.792,2.841,3.726L123.313,180.87c-3.919,3.648-6.447,8.53-7.163,13.829l-3.798,28.146
	   c-0.503,3.758-5.782,4.131-6.819,0.494l-14.607-51.325C89.253,166.16,91.691,159.907,96.869,156.711z"
							fill="#8d8d8d"
						/>
					</g>
				</svg></a
			>
		</li>
		<li>
			<a
				href="https://www.linkedin.com/company/digital-insight-games/"
				target="_blank"
				class="sns-linkedin"
				title="Open The Linkedin Link In A New Window"
			>
				<!--?xml version="1.0" encoding="iso-8859-1"?-->
				<!-- Generator: Adobe Illustrator 19.0.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
				<svg
					version="1.1"
					id="Layer_1"
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					x="0px"
					y="0px"
					viewBox="0 0 310 310"
					style="enable-background:new 0 0 310 310;"
					xml:space="preserve"
				>
					<g id="XMLID_801_">
						<path
							id="XMLID_802_"
							d="M72.16,99.73H9.927c-2.762,0-5,2.239-5,5v199.928c0,2.762,2.238,5,5,5H72.16c2.762,0,5-2.238,5-5V104.73
	   C77.16,101.969,74.922,99.73,72.16,99.73z"
							fill="#8d8d8d"
						/>
						<path
							id="XMLID_803_"
							d="M41.066,0.341C18.422,0.341,0,18.743,0,41.362C0,63.991,18.422,82.4,41.066,82.4
	   c22.626,0,41.033-18.41,41.033-41.038C82.1,18.743,63.692,0.341,41.066,0.341z"
							fill="#8d8d8d"
						/>
						<path
							id="XMLID_804_"
							d="M230.454,94.761c-24.995,0-43.472,10.745-54.679,22.954V104.73c0-2.761-2.238-5-5-5h-59.599
	   c-2.762,0-5,2.239-5,5v199.928c0,2.762,2.238,5,5,5h62.097c2.762,0,5-2.238,5-5v-98.918c0-33.333,9.054-46.319,32.29-46.319
	   c25.306,0,27.317,20.818,27.317,48.034v97.204c0,2.762,2.238,5,5,5H305c2.762,0,5-2.238,5-5V194.995
	   C310,145.43,300.549,94.761,230.454,94.761z"
							fill="#8d8d8d"
						/>
					</g>
				</svg></a
			>
		</li>
		<li>
			<a
				href="https://medium.com/DigitalInsightGames"
				target="_blank"
				class="sns-medium"
				title="Open The Medium Link In A New Window"
				><svg width="20px" height="20px" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"
					><path
						d="M18.75 5S18 5 18 5.75v8.5s0 .75.75.75H19v2h-6v-2h1V5.7h-.1L10.835 17H8.137L5.1 5.7H5V15h1v2H1v-2h.25S2 15 2 14.25v-8.5S2 5 1.25 5H1V3h6.634l2.327 8.66h.077L12.386 3H19v2h-.25z"
						fill="#8d8d8d"
					/></svg
				></a
			>
		</li>
	</ul>
</div>

<div class="offcanvas {endOpen}" toggle={toggleEnd} placement="end">
	<img on:click={toggleEnd} src={ico_close2} alt="" />
	<ul>
		<li on:click={toggleEnd}>
			<a href="/">Home</a>
		</li>
		<li on:click={toggleEnd}>
			<a href="/company">Company</a>
		</li>
		<li on:click={toggleEnd}>
			<a href="/team">Team</a>
		</li>
		<li on:click={toggleEnd}>
			<a href="/news">News</a>
		</li>
		<li on:click={toggleEnd}>
			<a href="/careers">Careers</a>
		</li>
		<li on:click={toggleEnd}>
			<a href="https://cloudcastles.gg/">Games</a>
		</li>
	</ul>
</div>

<style>
	header {
		padding: 15px 0;
		position: fixed;
		width: 100%;
		top: 0;
		z-index: 999;
		transition: 0.5s;
	}
	.main-menu li {
		margin-left: 50px;
		text-transform: uppercase;
	}
	.main-menu a {
		text-transform: uppercase;
		font-size: 19px;
	}
	.normal-state li a {
		color: #fff !important;
	}
	.sticky-nav li a {
		color: #000 !important;
	}
</style>
