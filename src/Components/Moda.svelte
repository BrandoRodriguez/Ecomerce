
<script>
import Modal from "./Modal.svelte";
 let showModal = false;
</script>





<button  on:click="{() => showModal = true}">
	show modal
</button>

{#if showModal}
	<Modal on:close="{() => showModal = false}">
	
		<a href="https://www.merriam-webster.com/dictionary/modal">merriam-webster.com</a>
	</Modal>
{/if}
