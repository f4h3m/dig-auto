<script>
	export let newsImg;
	export let newsTitle;
	export let newsDesc;
	export let newsDate;
	export let newsUrl;
</script>

<div
	class="single_blog wow fadeInUp"
	data-wow-duration="1s"
	data-wow-delay="0.5s"
	data-wow-offset="100"
>
	<a target="_blank" href={newsUrl}><img class="img-fluid" src={newsImg} alt="" />{newsTitle}</a>
	<p>{newsDesc}</p>
	<h5>{newsDate}</h5>
</div>

<style>
	/* News start */

	.single_blog a {
		display: block;
		font-size: 24px;
		color: var(--black);
		font-weight: 600;
		line-height: 1.4;
		margin-bottom: 10px;
		text-overflow: ellipsis;
		display: -webkit-box;
		-webkit-line-clamp: 3;
		-webkit-box-orient: vertical;
		word-break: keep-all;
		overflow: hidden;
	}

	.single_blog a img {
		border-radius: 20px;
		margin-bottom: 25px;
	}

	.single_blog p {
		color: #999;
		font-size: 17px;
		margin-bottom: 20px;
		text-overflow: ellipsis;
		display: -webkit-box;
		-webkit-line-clamp: 3;
		-webkit-box-orient: vertical;
		word-break: keep-all;
		overflow: hidden;
	}

	.single_blog h5 {
		font-size: 14px;
		font-weight: 300;
		color: #999;
	}
	/* News end  */
</style>
