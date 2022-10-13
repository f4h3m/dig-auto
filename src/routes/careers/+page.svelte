<script>
	// import assets
	import company_video_banner from '$lib/images/company-video-banner.jpg';
	import company_video from '$lib/video/careers-vid-bg.mp4';
	import job_icon from '$lib/images/job.png';

	function scrollIntoView({ target }) {
		const el = document.querySelector(target.getAttribute('href'));
		if (!el) return;
		el.scrollIntoView({
			behavior: 'smooth'
		});
	}

	// json data
	import careers from '$lib/data/careers.json';
</script>

<!--Hero Area Start-->
<section
	class="careers-hero-section section-gap d-flex align-items-center fix overlay"
	id="careers-hero-section"
>
	<video poster={company_video_banner} src={company_video} muted autoplay loop />
	<div class="container">
		<div class="row">
			<div class="col-lg-7">
				<h1>COME COLLABORATE WITH DIG</h1>
				<h4>
					We strive to achieve high standards, and are actively creating a culture based on teamwork
					and growth. A collaborative community, creating more than games. Join us in creating
					magical experiences for people to enjoy.
				</h4>
				<ul>
					<li>&#9733; Highly competitive Comp package</li>
					<li>&#9733; Full healthcare and other benefits</li>
					<li>&#9733; Communication/WFH stipend</li>
					<li>&#9733; Fully remote; work where you choose</li>
					<li>&#9733; Standard paid time off</li>
				</ul>
				<a class="btn_primary" href="#openjobs-section" on:click|preventDefault={scrollIntoView}
					>Explore Jobs</a
				>
			</div>
		</div>
	</div>
</section>
<!--Hero Area end-->
<div class="open-jobs-section section-gap section_padding" id="openjobs-section">
	<div class="container">
		<div class="row">
			<div class="col-lg-12">
				<div class="section_title">
					<h2>Open Jobs</h2>
				</div>
			</div>
		</div>
		<div class="row">
			{#each careers as career}
				<div class="col-md-4">
					<div class="single-jobs">
						<a class="d-flex align-items-center" href={career.link}>
							<img src={job_icon} alt="" />
							<span>{career.name}</span>
						</a>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>

<style>
	/* careers hero_area css */

	.careers-hero-section {
		z-index: 1;
		height: 850px;
		color: var(--white);
	}

	.careers-hero-section video {
		position: absolute;
		top: 0;
		bottom: 0;
		left: 0;
		z-index: -1;
		width: 100%;
	}

	.careers-hero-section h1 {
		font-size: 36px;
	}

	.careers-hero-section h4 {
		font-size: 24px;
		font-weight: 300;
		line-height: 1.4;
		margin-bottom: 30px;
	}

	.careers-hero-section ul li {
		color: var(--white);
		font-size: 20px;
		line-height: 27px;
		padding: 5px 0px;
		font-weight: 300;
	}

	.careers-hero-section .btn_primary {
		margin-top: 30px;
	}
	/* careers hero area end  */
	/* single-jobs start*/

	.single-jobs img {
		width: 30px;
		margin-right: 10px;
	}

	.single-jobs a {
		background: #f6f6f6;
		font-size: 18px;
		padding: 10px;
		margin-bottom: 10px;
		cursor: pointer;
		transition: 0.5s;
	}

	.single-jobs a:hover {
		background: var(--primary);
	}

	.single-jobs a span {
		color: #000 !important;
	}

	.single-jobs ul li a {
		display: block;
	}

	.single-jobs ul li a:hover {
		color: #000;
	}

	.single-jobs ul li img {
		width: 24px;
		margin-right: 4px;
	}
	/* single-jobs end*/
	@media (max-width: 575px) {
		.careers-hero-section {
			padding: 300px 0 !important;
		}
		.careers-hero-section h4 {
			font-size: 26px;
		}
		.careers-hero-section h4 {
			font-size: 14px;
		}
	}
</style>
