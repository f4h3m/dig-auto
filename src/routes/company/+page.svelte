<script>
	import company_video_banner from '$lib/images/company-video-banner.jpg';
	import company_video_banner_video from '$lib/video/company-video.mp4';
	import ico_customer from '$lib/images/ico-customer.svg';
	import ico_teamwork from '$lib/images/ico-teamwork.svg';
	import ico_boldness from '$lib/images/ico-boldness.svg';
	import ico_results from '$lib/images/ico-results.svg';
	import ico_iteration from '$lib/images/ico-iteration.svg';
	import ico_community from '$lib/images/ico-community.svg';
	import ico_mail from '$lib/images/ico-mail.svg';
	import maps from '$lib/images/map.jpeg';
</script>

<section class="company-page-hero section-gap">
	<div class="container">
		<div class="row">
			<div class="col-md-12">
				<h1 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">Company</h1>
				<h4 class="wow fadeInUp" data-wow-duration="1s" data-wow-delay="0.5s" data-wow-offset="100">
					<span class="span-yellow">Digital Insight Games (DIG)</span> aims to build the world’s
					premier
					<span class="span-black">AAA Metaverse experience,</span>
					with the best-in-class/user friendly Tech platform for
					<span class="span-black">next gen in-game digital economy,</span> enabling digital asset ownership,
					transparency, accessibility, scalability, and security.
				</h4>
			</div>
		</div>
	</div>
</section>

<section class="video-section">
	<video poster={company_video_banner} src={company_video_banner_video} muted autoplay loop />
</section>

<section class="our-culture-section section-gap">
	<div class="container">
		<div class="row">
			<div class="col-md-12">
				<h2
					class="section-title wow fadeInUp"
					data-wow-duration="1s"
					data-wow-delay="0.5s"
					data-wow-offset="100"
				>
					Our Culture
				</h2>
			</div>
		</div>
		<div class="row">
			<div class="col-md-6">
				<div class="single-culture wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					<div class="d-flex align-items-center">
						<div class="culture-thumb">
							<img class="img-fluid" src={ico_customer} alt="" />
						</div>
						<h4>Customer(Gamers) First</h4>
					</div>
					<p>
						We are an independent games company formed by gamers and are in the business of
						producing as well as publishing fantastic games for fellow gamers.
					</p>
				</div>
			</div>
			<div class="col-md-6">
				<div class="single-culture wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					<div class="d-flex align-items-center">
						<div class="culture-thumb">
							<img class="img-fluid" src={ico_teamwork} alt="" />
						</div>
						<h4>Teamwork</h4>
					</div>
					<p>
						Making a great game involves highly collaborative efforts across functions and
						disciplines. We value all of our contributors, no matter the participation level, in
						making our end product possible, that is a fantastically fun game to play.
					</p>
				</div>
			</div>
			<div class="col-md-6">
				<div class="single-culture wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					<div class="d-flex align-items-center">
						<div class="culture-thumb">
							<img class="img-fluid" src={ico_boldness} alt="" />
						</div>
						<h4>Boldness</h4>
					</div>
					<p>
						We look for team members who challenge the status quo and seek to innovate across key
						departments in the organization. We strive to invent something new every day.
					</p>
				</div>
			</div>
			<div class="col-md-6">
				<div class="single-culture wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					<div class="d-flex align-items-center">
						<div class="culture-thumb">
							<img class="img-fluid" src={ico_results} alt="" />
						</div>
						<h4>Results Oriented</h4>
					</div>
					<p>
						We live and die by the quality of our work and seek to produce great games for our fans.
						We take the quality of our games seriously, and disappointment by our customers is not
						an option.
					</p>
				</div>
			</div>
			<div class="col-md-6">
				<div class="single-culture wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					<div class="d-flex align-items-center">
						<div class="culture-thumb">
							<img class="img-fluid" src={ico_iteration} alt="" />
						</div>
						<h4>Iteration</h4>
					</div>
					<p>
						We aim to tweak and change any imperfections into perfection over time. We aim to
						iterate our way to success by finding that secret sauce. All we ask is for our loyal
						gamers to stay with us and lend us the support we need to make the long journey
						possible. Together, we are going to make it!
					</p>
				</div>
			</div>
			<div class="col-md-6">
				<div class="single-culture wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					<div class="d-flex align-items-center">
						<div class="culture-thumb">
							<img class="img-fluid" src={ico_community} alt="" />
						</div>
						<h4>Community</h4>
					</div>
					<p>
						We seek to pioneer a Games-as-a-Service/Live Service 2.0 model where we aim to build a
						game in conjunction with our community. We plan to integrate player community feedback
						across all stages including during both game development phase as well as post-launch
						phase. We’ll iterate live with our community even during the design and production
						phases! We’re all in this together, both inside and outside the company.
					</p>
				</div>
			</div>
		</div>
	</div>
</section>

<section class="contact-section section-gap">
	<div class="container">
		<div class="row">
			<div class="col-lg-8 col-md-12">
				<h2 class="section-title wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					Contact
				</h2>
				<h4 class="wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
					DIG is a remote-first and decentralized company with regional bases in Vancouver (Canada),
					Los Angeles, San Francisco, Austin, and New York, USA.
				</h4>
				<a
					class="mail-address wow fadeInUp"
					data-wow-duration="1s"
					data-wow-offset="100"
					href="mailto:info@digitalinsightgames.com"
				>
					<img src={ico_mail} alt="" />
					<span>info@digitalinsightgames.com</span>
				</a>
			</div>
		</div>
		<div class="row justify-content-center">
			<div class="col-lg-8 col-md-12">
				<div class="text-center">
					<img
						class="img-fluid map-image wow fadeInUp"
						data-wow-duration="1s"
						data-wow-delay="0.5s"
						data-wow-offset="100"
						src={maps}
						alt=""
					/>
				</div>
			</div>
		</div>
	</div>
</section>

<style>
	.company-page-hero {
		padding-top: 200px;
	}

	.company-page-hero h1 {
		font-size: 80px;
		font-weight: 700;
		color: #000;
	}
	.company-page-hero h4 {
		font-size: 48px;
		font-weight: 100;
		color: #000;
	}

	.company-page-hero h4 span {
		font-weight: 700;
	}

	.company-page-hero h4 .span-yellow {
		color: #fece4f;
	}

	.video-section video {
		width: 100%;
		position: absolute;
		bottom: 0;
		left: 0;
	}

	.video-section {
		position: relative;
		overflow: hidden;
		height: 650px;
	}

	.single-culture {
		margin-top: 60px;
	}

	.single-culture .culture-thumb {
		width: 80px;
		margin-right: 10px;
		display: block;
	}

	.single-culture h4 {
		margin-bottom: 0;
		font-weight: 700;
		font-size: 19px;
	}

	.single-culture p {
		font-size: 18px;
		margin-top: 10px;
		font-weight: 300;
	}
	.contact-section h4 {
		font-size: 32px;
		font-weight: 300;
	}
	.mail-address {
		margin-top: 30px;
		display: flex;
		align-items: center;
	}

	.mail-address span {
		font-weight: 700;
		font-size: 22px;
		padding-left: 10px;
		color: #000;
	}
	.map-image {
		margin-top: 40px;
		/* max-width: 1000px; */
	}

	@media (max-width: 767px) {
		.video-section {
			height: 400px;
		}
		.contact-section {
			padding-top: 0;
		}
	}
	@media (max-width: 575px) {
		.company-page-hero {
			padding-bottom: 0;
		}
		.company-page-hero h4 {
			font-size: 25px;
		}
	}
</style>
