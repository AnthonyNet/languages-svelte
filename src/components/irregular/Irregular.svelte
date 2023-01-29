<script lang="ts">
	import Stars from '../card/Stars.svelte';
	export let myData: any;

	const styles = {
		section:
			'section_Responsive flex justify-center items-center w-full h-[91vh] responsiveSection',
		section_div:
			'max-w-sm card my-8 xl:my-0 border-4 border-double border-blue-700 rounded-lg shadow-xl shadow-slate-600 text-center',
		score_div: 'py-3 px-6 border-b border-gray-300',
		stars__div: 'flex items-center justify-center py-3 border-b border-gray-300 text-yellow-500',
		btn_div: 'border-t border-gray-300 text-gray-600',
		h5: 'text-xl dark:bg-black font-medium mb-2 border-b border-gray-300',
		ul: 'flex flex-col justify-around text-center mb-2'
	};
	let stars = [1, 2];
</script>

<section class={styles.section}>
	<div class={styles.section_div}>
		<div class={styles.score_div}>
			Celkové skóre: <span>0</span>
		</div>
		<div class={styles.score_div}>
			Momentální skóre: <span>0</span>
		</div>

		<div class={styles.stars__div}>
			{#each stars as star}
				<Stars />
			{/each}
		</div>

		<div class="px-6 inputs">
			<h5 class={styles.h5}>cz</h5>

			<ul class={styles.ul}>INPUTS</ul>

			<div class={styles.btn_div}>
				<button />
			</div>
		</div>

		<div class={styles.btn_div}>
			<button />

			hints
		</div>
	</div>
</section>
