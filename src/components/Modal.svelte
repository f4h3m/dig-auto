<script>
	export let TeamMemberName;
	export let TeamMemberDesignation;
	export let TeamMemberLinkedin;
	export let TeamMemberDetails;

	import close_btn from '$lib/images/ico-close.svg';
	import linkedin_icon from '$lib/images/linkdon-icon.png';
</script>

<div on:click|self class="modal">
	<div class="modal-content" on:click>
		<div on:click class="close-btn text-right">
			<img src={close_btn} alt="" />
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
		<p>{TeamMemberDetails}</p>
	</div>
</div>
