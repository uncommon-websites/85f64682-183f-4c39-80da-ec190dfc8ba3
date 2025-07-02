<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
	testimonials={[
		{
			name: "Linh Dai",
			position: "Founder & Creative Lead",
			company: "Snaplight Agency",
			quote:
				"I used to spend 3–4 hours a day just trying to stay on top of email. Serif now does 90% of that for me—and we closed the last quarter up 27% in client volume without adding headcount.",
			image: "/generated/image-a-professional-headshot-of-a-hispanic-wo.webp"
		},
		{
			name: "Ernesto Ruiz",
			position: "VP of Growth",
			company: "Assort Health",
			quote:
				"With Serif running follow-ups automatically on behalf of our sales team, we save over 180 hours a month and cut our sales cycle by 9%. The ROI is instant.",
			image: "/generated/image-a-professional-headshot-of-a-black-man-e.webp"
		},
		{
			name: "Alex Stattner",
			position: "Top Business Broker",
			company: "U.S. Business Brokerage",
			quote:
				"Serif helped me streamline buyer outreach, seller updates, and due diligence follow-ups in one place. I now manage over 150+ emails a day solo and still have time to close 6-figure deals weekly.",
			image: "/generated/image-a-professional-headshot-of-an-asian-woma.webp"
		}
	]}
/>

<CallToAction
	title="The top professionals already use Serif. Now it's your turn."
	subtitle="Experience email freedom now"
	description="Join the pros saving hours every day, with 1M+ emails drafted and a 59% success rate. Your assistant is standing by."
	imageSrc="/generated/image-a-professional-business-owner-sitting-at.webp"
	callsToAction={[
		{
			href: "/signup",
			label: "Start free trial",
			variant: "primary"
		},
		{
			href: "/demo",
			label: "See how it works",
			variant: "secondary"
		}
	]}
/>
