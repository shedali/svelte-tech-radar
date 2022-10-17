<script>
	import { onMount } from 'svelte';

	onMount(() => {
		radar_visualization({
			svg_id: 'radar',
			width: 1450,
			height: 1000,
			colors: {
				background: '#fff',
				grid: '#bbb',
				inactive: '#ddd'
			},
			title: 'Tech Radar',
			quadrants: [
				{ name: 'Languages' },
				{ name: 'Infrastructure' },
				{ name: 'Datastores' },
				{ name: 'Data Management' }
			],
			rings: [
				{ name: 'ADOPT', color: '#93c47d' },
				{ name: 'TRIAL', color: '#93d2c2' },
				{ name: 'ASSESS', color: '#fbdb84' },
				{ name: 'HOLD', color: '#efafa9' }
			],
			print_layout: true,
			// zoomed_quadrant: 0,
			//ENTRIES
			entries: [
				// {
				// 	quadrant: 3,
				// 	ring: 2,
				// 	label: 'Tailwind',
				// 	active: true,
				// 	moved: 0
				// },
				// {
				// 	quadrant: 3,
				// 	ring: 2,
				// 	label: 'Vite',
				// 	active: true,
				// 	moved: 0
				// },
				// {
				// 	quadrant: 3,
				// 	ring: 2,
				// 	label: 'Sveltekit',
				// 	active: true,
				// 	moved: 0
				// }
			]
			//ENTRIES
		});
	});
</script>

<svg id="radar"></svg>
