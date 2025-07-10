<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
	import ImageSection from "$lib/components/layout/ImageSection.svelte";
</script>

<CustomerCardHero
	title="Your AI Executive Assistant for Business Excellence"
	centered={false}
	customers={[
		{
			name: "Sarah Chen",
			position: "Business Broker",
			imageSrc: "/generated/image-a-confident-businesswoman-dressed-in-a-s.webp"
		},
		{
			name: "Michael Rodriguez", 
			position: "Agency Owner",
			imageSrc: "/generated/image-a-focused-businessman-in-a-tailored-suit.webp"
		},
		{
			name: "Jennifer Walsh",
			position: "Sales Manager", 
			imageSrc: "/generated/image-a-dynamic-businesswoman-in-a-sharp-profe.webp"
		},
		{
			name: "David Park",
			position: "Executive",
			imageSrc: "/generated/image-a-charismatic-businessman-in-a-modern-wo.webp"
		},
		{
			name: "Lisa Thompson",
			position: "Real Estate Broker",
			imageSrc: "/generated/image-a-poised-businesswoman-in-a-chic-profess.webp"
		}
	]}
/>
<ImageSection 
	imageSrc="/uploaded/1752134372704-cfzfc7q.jpg"
	alt="Historical map of northern European coastal regions"
/>
<LogoScroller 
	label="Trusted by industry leaders" 
	logoUrls={[
		'https://logo.clearbit.com/remax.com',
		'https://logo.clearbit.com/salesforce.com',
		'https://logo.clearbit.com/hubspot.com',
		'https://logo.clearbit.com/shopify.com'
	]}
/>

<Summary
	title="What we do"
	text="Serif is your AI-powered executive assistant that transforms how people-facing professionals manage their business communication. We auto-draft emails in seconds, build persistent knowledge bases, and help you achieve true email freedom. Join thousands of professionals who save 10+ hours weekly with our intelligent automation tools."
/>

<Testimonials
	testimonials={[
		{
			name: "Mario Cervetti",
			position: "Founder",
			company: "Assort Health",
			quote:
				"Serif saved our sales team 190 hours monthly and helped us close deals 9% faster. The ROI was immediate - we recovered our investment in the first week alone.",
			image:
				"/generated/image-a-professional-businessman-wearing-a-sle.webp"
		},
		{
			name: "Reena Zhang",
			position: "Top Business Broker",
			company: "National Transactions Group",
			quote:
				"Managing 150+ emails daily was consuming my life. Now Serif saves me 10+ hours every week while reducing the risk of missing critical client communications.",
			image:
				"/generated/image-a-professional-businesswoman-in-a-contem.webp"
		},
		{
			name: "Felix Monroe",
			position: "Owner",
			company: "HM Web Agency",
			quote:
				"Serif paid for itself within days. My agency now closes deals 2x faster and I've eliminated the money drain of missed follow-ups and delayed responses.",
			image:
				"/generated/image-a-professional-businessman-in-business-c.webp"
		}
	]}
/>

<Features
	title="Why professionals choose Serif"
	subtitle="The AI executive assistant that transforms how you work"
	features={[
		{
			title: "AI email automation",
			description: "Save 10+ hours weekly with intelligent email drafting that learns your voice and handles responses automatically."
		},
		{
			title: "24/7 executive assistant",
			description: "Your AI assistant works around the clock, managing conversations and keeping deals moving even while you sleep."
		},
		{
			title: "Persistent knowledge base",
			description: "Every interaction builds your business memory - SOPs, relationships, and preferences that make each response smarter."
		},
		{
			title: "Enterprise-grade security",
			description: "SOC 2 Type 2 compliant with encrypted data at rest, ensuring your emails never train general AI models."
		},
		{
			title: "Seamless integrations",
			description: "Works perfectly with Gmail and Outlook, automatically labeling emails and maintaining your existing workflow."
		},
		{
			title: "Team collaboration",
			description: "Shared knowledge bases and playbooks ensure consistent communication across your entire organization."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Email overflow management",
			description: "When your inbox becomes overwhelming and critical emails get buried, Serif's AI triages everything instantly, auto-drafts responses, and ensures no important communication falls through the cracks.",
			image: "/generated/image-a-group-of-business-executives-in-a-mode.webp",
			link: {
				href: "/use-cases/email-management",
				label: "Learn more"
			}
		},
		{
			title: "Sales acceleration",
			description: "Close deals 2x faster with instant follow-ups and contextual responses. Serif learns your sales process and maintains momentum across every prospect conversation without manual intervention.",
			image: "/generated/image-sales-professionals-gathered-in-a-stylis.webp",
			link: {
				href: "/use-cases/sales-acceleration",
				label: "Learn more"
			}
		},
		{
			title: "Business scaling support",
			description: "Scale your operations without scaling your administrative burden. Serif becomes your 24/7 executive assistant, managing increasing communication volume while you focus on growth.",
			image: "/generated/image-entrepreneurs-in-an-open-plan-workspace-.webp",
			link: {
				href: "/use-cases/business-scaling",
				label: "Learn more"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction 
	title="Stop drowning in email"
	subtitle="Start growing your business" 
	description="Join 1,000+ professionals who save 10+ hours weekly with Serif's AI-powered executive assistant. Auto-draft emails, manage conversations, and focus on what actually grows your business."
	imageSrc="/generated/image-a-happy-and-confident-business-professio.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Try Serif free",
			variant: "primary"
		},
		{
			href: "/demo",
			label: "See how it works",
			variant: "secondary"
		}
	]}
/>
