<script>
	import hero_bg_img from '$lib/images/hero-bg-img.jpg';
	import hero_bg_video from '$lib/video/hero-bg-video.mp4';
	import img_blizzard from '$lib/images/img-blizzard.png';
	import img_ea from '$lib/images/img-ea.png';
	import img_t2 from '$lib/images/img-t2.png';
	import img_tencent from '$lib/images/img-tencent.png';
	import img_ubisoft from '$lib/images/img-ubisoft.png';
	import circle_02 from '$lib/images/cicle_02.jpeg';
	import circle_02_video from '$lib/video/cicle_02.mp4';
	import circle_01_video from '$lib/video/cicle_01.mp4';
	import logo_hivemind from '$lib/images/logo-hivemind.png';
	import logo_hivemind_hover from '$lib/images/logo-hivemind-hover.png';
	import logo_griffin from '$lib/images/logo-griffin.png';
	import logo_griffin_hover from '$lib/images/logo-griffin-hover.png';
	import logo_hunt_normal from '$lib/images/logo-hunt-normal.png';
	import logo_hunt_hover from '$lib/images/logo-hunt-hover.png';
	import logo_rse_normal from '$lib/images/logo-rse-normal.png';
	import logo_rse_hover from '$lib/images/logo-rse-hover.png';
	import logo_heron_normal from '$lib/images/logo_heron_normal.png';
	import logo_heron_hover from '$lib/images/logo_heron_hover.png';

	// json data
	import news from '$lib/data/news.json';

	// components
	import NewsItem from '../components/NewsItem.svelte';
</script>

<!--Hero Area Start-->
<section class="hero-section d-flex align-items-center fix" id="hero-section">
	<video poster={hero_bg_img} autoplay loop muted playsinline webkit-playsinline>
		<source src={hero_bg_video} type="video/mp4" />
	</video>
	<div class="container">
		<div class="row">
			<div class="col-lg-6 hero-txt">
				<h1>
					<span class="wow slideInLeft" data-wow-duration="1.5s" data-wow-offset="100"
						>POWERED BY</span
					>
					<div
						class="wow slideInLeft"
						data-wow-duration="1.5s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						IMAGINATION
					</div>
				</h1>
				<p
					class="wow slideInLeft"
					data-wow-duration="2s"
					data-wow-delay="0.5s"
					data-wow-offset="100"
				>
					Digital Insight Games is a next-generation games studio founded by industry veterans.
					We're at the forefront of technology and digital economies, defining the future of
					world-class interactive entertainment.
				</p>
			</div>
		</div>
	</div>
</section>
<section class="team-section section-gap">
	<div class="container">
		<div class="row">
			<div class="col-lg-12">
				<div class="section_title">
					<h2 class="section-title wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
						Our Team is
					</h2>
				</div>
			</div>
		</div>
		<div class="row justify-content-center">
			<div class="col-lg-12">
				<p class="wow fadeInUp" data-wow-duration="1s" data-wow-delay="0.5s" data-wow-offset="100">
					Composed of individuals from leading globally renowned Games companies including
					Activision Blizzard, Electronic Arts, Take-Two, Tencent, Ubisoft as well as numerous
					others.
				</p>
				<div class="logo_list">
					<ul>
						<li>
							<img
								class="wow fadeInUp"
								data-wow-duration="1s"
								data-wow-offset="100"
								src={img_blizzard}
								alt=""
							/>
						</li>
						<li>
							<img
								class="wow fadeInDown"
								data-wow-duration="1s"
								data-wow-offset="100"
								src={img_ea}
								alt=""
							/>
						</li>
						<li>
							<img
								class="wow fadeInUp"
								data-wow-duration="1s"
								data-wow-offset="100"
								src={img_t2}
								alt=""
							/>
						</li>
						<li>
							<img class="wow fadeInDown" data-wow-offset="100" src={img_tencent} alt="" />
						</li>
						<li>
							<img
								class="wow fadeInUp"
								data-wow-duration="1s"
								data-wow-offset="100"
								src={img_ubisoft}
								alt=""
							/>
						</li>
					</ul>
				</div>
				<a class="btn_primary" href="/team">Team</a>
			</div>
		</div>
	</div>
</section>
<section class="core_pillars section-gap" id="">
	<div class="container">
		<!-- Section Title -->
		<div class="row">
			<div class="col-lg-12">
				<div class="section_title">
					<h2 class="section-title">
						<div class="wow slideInLeft" data-wow-duration="1.5s" data-wow-offset="100">
							Our Core Pillars &
						</div>
						<div class="wow slideInLeft" data-wow-duration="1.5s" data-wow-offset="100">
							Company Ethos
						</div>
					</h2>
				</div>
			</div>
		</div>
		<!-- Section Title -->
		<div class="row justify-content-center">
			<div class="col-lg-6">
				<div class="video_area">
					<div
						class="video_1 video_wraper wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						<video
							width="100%"
							height=""
							poster={circle_02}
							autoplay
							loop
							muted
							playsinline
							webkit-playsinline
						>
							<source src={circle_02_video} type="video/mp4" />
						</video>
					</div>
					<div
						class="video_2 video_wraper wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						<video
							width="100%"
							height=""
							poster={circle_02}
							autoplay
							loop
							muted
							playsinline
							webkit-playsinline
						>
							<source src={circle_01_video} type="video/mp4" />
						</video>
					</div>
				</div>
			</div>
			<div class="col-lg-6">
				<div class="text_area">
					<h3 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">Fun</h3>
					<p
						class="wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						Games are meant to be enjoyed.
					</p>
					<h3 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">Innovation</h3>
					<p
						class="wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						We strive to be at the forefront of what gamers want: Incredible gameplay, art, design,
						and technology.
					</p>
					<h3 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">Ownership</h3>
					<p
						class="wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						We believe gamers who are our loyal customers should have the ability to own any in-game
						digital items after spending time, energy, and money into the ecosystem. Residual value
						of any digital assets should be accrued to the player. We create games that empower
						players to own, buy, sell, trade, collect, and have control of their digital assets!
					</p>
					<h3 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">Transparency</h3>
					<p
						class="wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						We believe our customers should be engaged at every stage of the development process.
						Full game development cycles should be iterated live in partnership with our loyal
						gaming community.
					</p>
					<h3 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">Accessibility</h3>
					<p
						class="wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
					>
						We believe everyone in the world from all economic backgrounds should have the ability
						to enjoy our games. We aim to build a gaming platform that’s user-friendly, scalable,
						and safe. Our games are to be enjoyed by everyone.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>
<section class="investors section-gap" id="">
	<div class="container">
		<!-- Section Title -->
		<div class="row">
			<div class="col-lg-12">
				<div class="section_title">
					<h2 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">Investors</h2>
				</div>
			</div>
		</div>
		<!-- Section Title -->
		<div class="row justify-content-center">
			<div class="col-lg-10">
				<div class="row justify-content-center">
					<div class="col-lg-4">
						<a
							target="_blank"
							class="single_logo_box wow fadeInUp"
							data-wow-duration="1s"
							data-wow-offset="100"
							href="https://hivemindcapital.co/"
						>
							<img class="regular" src={logo_hivemind} alt="" />
							<img class="hover" src={logo_hivemind_hover} alt="" />
							<p>Hivemind Capital</p>
						</a>
					</div>
					<div class="col-lg-4">
						<a
							target="_blank"
							class="single_logo_box wow fadeInUp"
							data-wow-duration="1s"
							data-wow-offset="100"
							href="https://griffingp.com/"
						>
							<img class="regular" src={logo_griffin} alt="" />
							<img class="hover" src={logo_griffin_hover} alt="" />
							<p>Griffin Gaming Partners</p>
						</a>
					</div>
				</div>
			</div>
			<div class="top_bar separetor" />
			<div class="col-lg-10">
				<div class="row">
					<div class="col-lg-4">
						<a
							target="_blank"
							class="single_logo_box wow fadeInUp"
							data-wow-duration="1s"
							data-wow-offset="100"
							href="/"
						>
							<img class="regular" src={logo_hunt_normal} alt="" />
							<img class="hover" src={logo_hunt_hover} alt="" />
							<p>Hunt Technology Ventures</p>
						</a>
					</div>
					<div class="col-lg-4">
						<a
							target="_blank"
							class="single_logo_box wow fadeInUp"
							data-wow-duration="1s"
							data-wow-offset="100"
							href="https://rseventures.com/"
						>
							<img class="regular" src={logo_rse_normal} alt="" />
							<img class="hover" src={logo_rse_hover} alt="" />
							<p>RSE Ventures</p>
						</a>
					</div>
					<div class="col-lg-4">
						<a
							target="_blank"
							class="single_logo_box wow fadeInUp"
							data-wow-duration="1s"
							data-wow-offset="100"
							href="https://blueheronventures.com/"
						>
							<img class="regular" src={logo_heron_normal} alt="" />
							<img class="hover" src={logo_heron_hover} alt="" />
							<p>Blue Heron Ventures</p>
						</a>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
<section class="news section-gap">
	<div class="container">
		<!-- Section Title -->
		<div class="row">
			<div class="col-lg-12">
				<div class="section_title">
					<h2 class="section-title wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
						News
					</h2>
				</div>
			</div>
		</div>
		<div class="row">
			{#each news as single_news}
				<div class="col-md-3">
					<NewsItem
						newsImg={single_news.newsImg}
						newsTitle={single_news.newsTitle}
						newsDesc={single_news.newsDesc}
						newsDate={single_news.newsDate}
						newsUrl={single_news.newsUrl}
					/>
				</div>
			{/each}
			<div class="mx-auto">
				<a class="btn_primary" href="/news">News</a>
			</div>
		</div>
		<!-- Section Title -->
	</div>
</section>

<style>
	/* hero area css start */
	.hero-section {
		z-index: 1;
		color: var(--white);
		position: relative;
		height: 980px;
		overflow: hidden;
	}

	.hero-section:after {
		position: absolute;
		content: '';
		background-color: rgba(0, 0, 0, 0.8);
		height: 100%;
		width: 100%;
		z-index: 0;
		top: 0;
		left: 0;
		transition: 0.5s;
		opacity: 0.5;
	}

	.hero-txt {
		position: relative;
		z-index: 99;
	}

	.hero-txt p {
		width: 98%;
		font-size: 1.625rem !important;
	}

	.hero-section video {
		position: absolute;
		left: 0;
		top: 0;
		width: 100%;
	}

	.hero-section h1 {
		font-size: 98px;
		color: #fff;
		font-weight: 700;
		margin-bottom: 20px;
	}

	.hero-section h1 span {
		display: block;
		font-weight: 100;
		color: #fff;
	}

	.hero-section p {
		font-size: 18px;
		font-weight: 300;
		color: #fff;
	}
	/* hero area css end */
	/* Team Start */

	.team-section p {
		max-width: 820px;
		font-size: 26px;
		font-weight: 300;
		margin-bottom: 50px;
	}

	.logo_list ul li {
		display: inline-block;
		margin-right: 40px;
	}

	.logo_list ul li:last-child {
		margin-right: 0;
	}

	.logo_list ul li img {
		height: 50px;
	}

	.team-section a {
		margin-top: 40px;
	}
	/* Team End */
	/* core_pillars start */

	.core_pillars {
		background-color: #0c0c0c;
		color: var(--white);
	}

	.core_pillars h2 {
		color: var(--white) !important;
		margin: 0 0 50px 0;
	}

	.core_pillars h3 {
		color: var(--primary);
		font-weight: 300;
		font-size: 28px;
	}

	.core_pillars p {
		font-weight: 200;
		font-size: 18px;
		margin-bottom: 30px;
	}

	.video_area {
		display: flex;
		height: 100%;
		flex-direction: column;
		justify-content: center;
	}

	.video_wraper {
		border-radius: 50%;
		overflow: hidden;
	}

	.video_wraper video {
		border-radius: 50%;
	}

	.video_1 {
		margin-left: 15%;
		margin-bottom: 100px;
		width: 320px;
		height: 320px;
		margin: 0 auto;
	}

	.video_2 {
		width: 270px;
		height: 270px;
	}
	/* core_pillars end  */
	/* investors start */

	.investors {
		background-color: #0c0c0c;
		color: var(--white);
	}

	.investors .section_title h2 {
		color: var(--primary);
		max-width: 480px;
		margin: 0 0 50px 0;
		font-size: 64px;
		font-weight: 600;
	}

	.investors .single_logo_box {
		position: relative;
		display: block;
		transition: 0.5s;
	}

	.investors .single_logo_box img {
		position: absolute;
		top: 0;
		left: 50%;
		height: 100px;
		transition: 0.5s;
		transform: translateX(-50%);
	}

	.investors .regular {
		opacity: 1;
	}

	.investors .hover {
		opacity: 0;
	}

	.investors .single_logo_box:hover .hover {
		opacity: 1;
	}

	.investors .single_logo_box p {
		transition: 0.5s;
		color: var(--white);
		text-align: center;
		padding-top: 110px;
		font-size: 18px;
		font-weight: 300;
	}

	.investors .single_logo_box:hover p {
		color: var(--primary);
	}

	.investors .separetor {
		margin: 65px 0;
	}
	/* investors end  */
	@media (max-width: 1399px) {
		.hero-section h1 {
			font-size: 85px;
		}
	}
	@media (max-width: 1739px) {
		.hero-section video {
			width: auto !important;
			height: 100% !important;
		}
	}
	@media (max-width: 991px) {
		.investors h2 {
			text-align: center;
			max-width: 100% !important;
		}
	}
	@media (max-width: 767px) {
		.hero-section h1 {
			font-size: 55px;
		}
	}
	@media (max-width: 536px) {
		.core_pillars h2 {
			font-size: 35px;
		}
	}
</style>
