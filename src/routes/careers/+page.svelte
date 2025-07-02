<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "Shape the future of AI",
			description: "Work on cutting-edge AI technology that's already helped send 1 million emails and serves top professionals worldwide.",
			icon: IconBriefcase
		},
		{
			title: "Exponential growth opportunity",
			description: "Join a team scaling from 0 to $400K ARR in 5 months with 83.8% retention and massive expansion plans.",
			icon: IconUsers
		},
		{
			title: "Impact at scale",
			description: "Help people-facing professionals save hundreds of hours while building the business management platform of the future.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
		{
			name: "Sarah Kim",
			position: "Senior Software Engineer",
			company: "Engineering Team",
			quote:
				"Building AI that's already processed 1 million emails and maintains 83% retention is incredibly rewarding. The technical challenges of creating an executive assistant that truly understands business context push me to innovate every day, and our rapid growth from 0 to 400K ARR shows the real impact of our work.",
			image:
				"/generated/image-a-professional-headshot-of-an-asian-woma.webp"
		},
		{
			name: "Jordan Williams",
			position: "Product Manager",
			company: "Product Team",
			quote:
				"Working at Serif means building products that save professionals hundreds of hours while scaling from startup to enterprise in months, not years. The growth opportunities are incredible when you're helping create the future of AI business tools and seeing our 74% retention prove we're solving real problems.",
			image:
				"/generated/image-a-professional-headshot-of-a-black-man-w.webp"
		},
		{
			name: "Maria Rodriguez",
			position: "Marketing Director",
			company: "Marketing Team",
			quote:
				"The collaborative culture here is unlike anywhere I've worked - everyone from Kevin to the newest engineer is focused on our mission to give professionals email freedom. Marketing revolutionary AI technology that genuinely transforms how people work is both challenging and deeply fulfilling.",
			image:
				"/generated/image-a-professional-headshot-of-a-hispanic-wo.webp"
		}
	];

	const processSteps = [
		{
			step: 1,
			title: "Apply",
			description:
				"Send your resume and a brief note about why you want to help build the future of AI executive assistance. Show us what makes you excited about transforming how professionals work."
		},
		{
			step: 2,
			title: "Connect & explore",
			description: "We'll have an in-depth conversation about your experience, our mission to reach $1B, and how you can help us scale from 400K ARR to the next level."
		},
		{
			step: 3,
			title: "Start building",
			description: "Join Kevin and the team working on AI that saves professionals hundreds of hours and helps them run billion-dollar businesses with minimal overhead."
		}
	];

	const values = [
		{
			icon: IconHeart,
			title: "AI-first innovation",
			description: "We're building the future where AI becomes your most trusted business partner, starting with email freedom and expanding to full executive assistance."
		},
		{
			icon: IconUsers,
			title: "Customer obsession",
			description: "From top business brokers to healthcare teams, we're relentlessly focused on helping people-facing professionals reclaim their time and scale their success."
		},
		{
			icon: IconGlobe,
			title: "Rapid execution",
			description: "We move fast and think big - achieving 400K ARR in 5 months while maintaining 83.8% retention and planning our path to $1B."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Build the future of AI-powered business"
	subtitle="Join Serif and help people-facing professionals reclaim their time. We're creating the world's most intelligent executive assistant, and we need passionate innovators to make it happen."
	imageSrc="/generated/image-a-diverse-group-of-professionals-includi.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join Serif?" subtitle="Be part of the AI revolution transforming how professionals work" />

	<div class="mt-16 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<Culture {values} />

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Join the team</h2>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
