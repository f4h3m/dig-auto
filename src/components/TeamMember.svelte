<script>
	export let TeamMemberImg;
	export let TeamMemberName;
	export let TeamMemberDesignation;
	export let TeamMemberLinkedin;
	export let TeamMemberDetails;

	import Modal from '../components/Modal.svelte';
	import linkedin_icon from '$lib/images/linkdon-icon.png';

	// initialise modal state and content
	let showModal = false;
	let modalContent;

	// pass in component as parameter and toggle modal state
	function toggleModal() {
		showModal = !showModal;
	}
</script>

{#if showModal}
	<Modal
		on:click={toggleModal}
		{TeamMemberName}
		{TeamMemberDesignation}
		{TeamMemberLinkedin}
		{TeamMemberDetails}
	/>
{/if}

<div
	class="single-team wow fadeInUp"
	data-wow-duration="1s"
	data-wow-offset="100"
	on:click={() => toggleModal()}
>
	<div class="thumb-img">
		<img class="img-fluid" src={TeamMemberImg} alt="" />
	</div>
	<div class="details-wrap d-flex align-items-center justify-content-center">
		<div class="name-details">
			<h4>{TeamMemberName}</h4>
			<p>{TeamMemberDesignation}</p>
		</div>
		<span>
			<a href={TeamMemberLinkedin}>
				<img class="img-fluid" src={linkedin_icon} alt="" />
			</a>
		</span>
	</div>
</div>

<style>
	.single-team {
		margin-top: 40px;
	}
	.single-team:hover {
		cursor: pointer;
	}
	.single-team .thumb-img {
		border-radius: 20px;
		overflow: hidden;
		margin-bottom: 20px;
		position: relative;
	}

	.thumb-img:before {
		content: '';
		display: inline-block;
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		left: 0;
		background: #ffcc3e66;
		opacity: 0;
		transition: 0.5s;
	}

	.single-team:hover .thumb-img:before {
		opacity: 1;
	}

	.details-wrap span a {
		width: 35px;
		display: inline-block;
	}
	.details-wrap h4 {
		font-weight: 700;
		font-size: 18px;
		margin-bottom: 5px;
	}

	.details-wrap span {
		border-left: 1px solid #ccc;
		padding-left: 30px;
	}
	.details-wrap p {
		margin-bottom: 0;
	}

	.name-details {
		padding-right: 30px;
	}

	@media (max-width: 991px) and (min-width: 768px) {
		.name-details {
			padding-right: 10px;
		}
		.details-wrap span {
			padding-left: 10px;
		}
	}
</style>
