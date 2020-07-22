<script>
	import ContactCard from './ContactCard.svelte'

	let name = "Name";
	let jobTitle = "Title";
	let description = "Desc";
	let imageUrl = "https://image.shutterstock.com/image-vector/person-icon-260nw-282598823.jpg";

	let done = false;

	function addContact(){
		done = true;
	}
</script>

	<div id="form">
		<div>
			<input type="text" bind:value="{name}" id="name"/>
		</div>
		<div>
			<input type="text" bind:value="{jobTitle}" id="jobTitle"/>
		</div>
		<div>
			<input type="text" bind:value="{imageUrl}" id="imageUrl"/>
		</div>
		<div>
			<input type="text" bind:value="{description}" id="description"/>
		</div>
	</div>
	<button on:click="{addContact}">Add Contact Card</button>


	{#if done}

	<ContactCard userName="{name}" jobTitle="{jobTitle}" imageUrl="{imageUrl}" description="{description}" />

	{/if}

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>