<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";

	// Icons
	import IconSearch from "~icons/lucide/search";
	import IconClock from "~icons/lucide/clock";
	import IconTrendingDown from "~icons/lucide/trending-down";
	import IconHandshake from "~icons/lucide/handshake";
	import IconBarChart from "~icons/lucide/bar-chart-3";
	import IconZap from "~icons/lucide/zap";
</script>

<Hero
	title="All your dental supplies,"
	subtitle="one effortless search"
	imageSrc="/generated/image-medium-wide-environmental-documentary-ph.webp"
	centered={false}
	callsToAction={[
		{
			href: "/contact",
			label: "Get started"
		},
		{
			href: "/about",
			label: "Learn more"
		}
	]}
/>
<LogoScroller
	label="Trusted by dental practices across Belgium"
	logoUrls={[
		'https://cdn.brandfetch.io/tandartspraktijk.nl/w/400/h/400/logo',
		'https://cdn.brandfetch.io/dentalclinic.be/w/400/h/400/logo',
		'https://cdn.brandfetch.io/smilecenter.be/w/400/h/400/logo',
		'https://cdn.brandfetch.io/orthocare.be/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="Everything you need"
	subtitle="Order dental supplies the way it should be"
	features={[
		{
			title: "Search across all suppliers",
			description:
				"Find any product instantly across 12+ trusted suppliers including Henry Schein, ADT, and Dental Addict without opening multiple browser tabs.",
			icon: IconSearch
		},
		{
			title: "Save hours every week",
			description:
				"Stop wasting time comparing prices and stock availability. Spend more time with patients and less time ordering supplies.",
			icon: IconClock
		},
		{
			title: "See your best prices",
			description:
				"View real-time pricing with your existing negotiated discounts and account-specific terms, so you always get the deal you earned.",
			icon: IconTrendingDown
		},
		{
			title: "Keep your trusted partners",
			description:
				"We're not a supplier, we're a search tool that works with your existing relationships, prices, and payment terms.",
			icon: IconHandshake
		},
		{
			title: "Understand your spending",
			description:
				"Track monthly supply costs and discover optimization opportunities with clear insights into your purchasing patterns.",
			icon: IconBarChart
		},
		{
			title: "Order in one click",
			description:
				"Place orders across multiple suppliers simultaneously with a single checkout, making restocking as simple as turning on the light.",
			icon: IconZap
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
