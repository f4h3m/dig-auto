<script>
	// json data
	import team_founders from '$lib/data/team_founders.json';
	import team_leaderships from '$lib/data/team_leaderships.json';
	import team_artdesigns from '$lib/data/team_artdesigns.json';
	import team_tech from '$lib/data/team_tech.json';
	import team_businessOps from '$lib/data/team_businessOps.json';
	import team_community from '$lib/data/team_community.json';
	import team_advisory from '$lib/data/team_advisory.json';

	// components
	import TeamMember from '../../components/TeamMember.svelte';
</script>

<div class="team-page-hero">
	<div class="container">
		<div class="row">
			<div class="col-md-12">
				<h1 class="wow fadeInUp text-center" data-wow-duration="1s" data-wow-offset="100">Team</h1>
			</div>
		</div>
	</div>
</div>

<div class="founders-section">
	<div class="container">
		<div class="row justify-content-center">
			<h2 class="team-title  wow fadeInUp" data-wow-duration="1s" data-wow-offset="100">
				Founders
			</h2>
			{#each team_founders as team_founder}
				<div class="col-md-4">
					<TeamMember
						TeamMemberImg={team_founder.TeamMemberImg}
						TeamMemberName={team_founder.name}
						TeamMemberDesignation={team_founder.designation}
						TeamMemberLinkedin={team_founder.linkedin_profile}
						TeamMemberDetails={team_founder.TeamMemberDetails}
					/>
				</div>
			{/each}
		</div>
	</div>
</div>

<div class="leadership-section">
	<div class="container">
		<div class="row">
			<h2 class="team-title">Leadership Team</h2>
			{#each team_leaderships as team_leadership}
				<div class="col-md-4">
					<TeamMember
						TeamMemberImg={team_leadership.TeamMemberImg}
						TeamMemberName={team_leadership.name}
						TeamMemberDesignation={team_leadership.designation}
						TeamMemberLinkedin={team_leadership.linkedin_profile}
						TeamMemberDetails={team_leadership.TeamMemberDetails}
					/>
				</div>
			{/each}
		</div>
	</div>
</div>

<div class="team-section">
	<div class="container">
		<div class="row">
			<h2 class="team-title">ART & DESIGN</h2>
			{#each team_artdesigns as team_artdesign}
				<div class="col-md-4">
					<div class="single-team-two">
						<h4>{team_artdesign.name}</h4>
						<p>{team_artdesign.designation}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>

<div class="team-section">
	<div class="container">
		<div class="row">
			<h2 class="team-title">ENGINEERING & TECH</h2>
			{#each team_tech as team_tech_single}
				<div class="col-md-4">
					<div class="single-team-two">
						<h4>{team_tech_single.name}</h4>
						<p>{team_tech_single.designation}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>

<div class="team-section">
	<div class="container">
		<div class="row">
			<h2 class="team-title">BUSINESS OPERATIONS</h2>
			{#each team_businessOps as team_businessOp}
				<div class="col-md-4">
					<div class="single-team-two">
						<h4>{team_businessOp.name}</h4>
						<p>{team_businessOp.designation}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>

<div class="team-section">
	<div class="container">
		<div class="row">
			<h2 class="team-title">COMMUNITY</h2>
			{#each team_community as team_community_single}
				<div class="col-md-4">
					<div class="single-team-two">
						<h4>{team_community_single.name}</h4>
						<p>{team_community_single.designation}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>

<div class="team-section">
	<div class="container">
		<div class="row">
			<h2 class="team-title">ADVISORY</h2>
			{#each team_advisory as team_advisory_single}
				<div class="col-md-4">
					<div class="single-team-two">
						<h4>{team_advisory_single.name}</h4>
						<p>{team_advisory_single.designation}</p>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>

<style>
	.leadership-section {
		padding-bottom: 100px;
	}

	.founders-section {
		padding-bottom: 180px;
	}

	.team-section {
		padding-bottom: 100px;
	}

	.team-page-hero {
		padding-top: 200px;
		padding-bottom: 50px;
	}
	.team-page-hero h1 {
		font-size: 80px;
		font-weight: 700;
	}
	.team-title {
		font-size: 32px;
		font-weight: 700;
		color: var(--primary);
	}

	.founders-section {
		padding-bottom: 180px;
	}

	.team-section {
		padding-bottom: 100px;
	}

	.single-team-two {
		margin-top: 30px;
		background: #e8e8e8;
		border-radius: 20px;
		padding: 30px 28px;
		text-align: center;
	}

	.single-team-two h4 {
		margin-bottom: 10px;
		font-size: 18px;
		font-weight: 700;
	}

	.single-team-two p {
		margin-bottom: 0px;
	}
</style>
