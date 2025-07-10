<script lang="ts">
	type Props = {
		imageSrc: string;
		alt?: string;
	};
	let { imageSrc, alt = '' }: Props = $props();
</script>

<section class="section-py section-px">
	<div class="container mx-auto">
		<div class="flex justify-center">
			<img 
				src={imageSrc} 
				{alt}
				class="w-full max-w-4xl h-auto object-contain"
			/>
		</div>
	</div>
</section>