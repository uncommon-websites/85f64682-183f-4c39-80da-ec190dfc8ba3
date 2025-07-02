<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Email freedom",
			description: "We believe professionals deserve to focus on what matters most, not inbox management."
		},
		{
			title: "Privacy first",
			description: "Your emails are never stored on our servers or used to train AI models. Security is core to our design."
		},
		{
			title: "Human-centered AI",
			description: "We build AI that amplifies human potential rather than replacing it, creating true partnership."
		}
	];
</script>

<SecondaryHero
	title="Empowering professionals with AI"
	subtitle="Your 24/7 executive assistant for email freedom"
	imageSrc="/mockups/airport-screen-1751487502252.png"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Kevin started Serif with a simple but urgent problem—email was eating his days alive. As a founder and people-facing professional himself, he watched countless hours vanish into writing replies, managing follow-ups, and organizing scattered knowledge. He didn't need a better email app. He needed an actual assistant. But for most solo professionals and small teams, that kind of help just wasn't accessible.",
		"So he set out to build it—creating Serif as a true executive assistant powered by AI. One that could understand your business, draft emails, handle back-and-forths, and free up your schedule. In just 5 months, Serif grew to $400K ARR, powered by an unheard-of 59% email acceptance rate and 83.8% month-one retention. Serif worked—and people started telling others. The viral word of mouth filled early growth without burning a single marketing dollar on paid ads.",
		"Now, Serif powers thousands of inboxes across industries—from the country's top business broker to fast-growing agencies and B2B sales teams. Customers have sent over 1 million emails with Serif, making only light edits before hitting send. And they're saving hundreds of hours every week getting out of email and back to running their business. For Kevin, the vision stays the same: make inboxes feel lighter, make decisions faster, and help people finally achieve true email freedom."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Meet the founder."
	subtitle="Building email freedom for professionals everywhere."
	stakeholders={[
		{
			name: "Kevin",
			position: "Founder & CEO",
			bio: "Kevin built Serif to solve his own email overwhelm problem, creating an AI executive assistant that helps people-facing professionals reclaim their time.",
			image: "/generated/image-a-professional-headshot-of-a-business-fo.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready for email freedom?"
	subtitle="Join thousands of professionals"
	description="Experience the AI assistant that saves hours every week and transforms how you manage your inbox. Start your journey to true email freedom today."
/>
