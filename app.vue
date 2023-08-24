<template>
	<NuxtLayout>
		<NuxtPage />
	</NuxtLayout>
</template>

<script setup lang="ts">
useHead({
	script: [
		{
			innerHTML: `
            window.dataLayer = window.dataLayer || [];
            function gtag() { dataLayer.push(arguments); }
            gtag('js', new Date());

            gtag('config', 'G-65GTQ707LB');
        `
		},
		{ src: 'https://www.googletagmanager.com/gtag/js?id=G-65GTQ707LB', async: true }
	]
});
useSeoMeta({
	title: 'Nohooks | Webhooks for platforms with no webhooks',
	ogTitle: 'Nohooks | Webhooks for platforms with no webhooks',
	twitterTitle: 'Nohooks | Webhooks for platforms with no webhooks',
	description: 'Nohooks is a service that offers webhooks functionality on platforms without native webhooks support. Developers can receive real-time notifications of events from supported apps. Powered by Convoy.',
	ogDescription: 'Nohooks is a service that offers webhooks functionality on platforms without native webhooks support. Developers can receive real-time notifications of events from supported apps. Powered by Convoy.',
	twitterDescription: 'Nohooks is a service that offers webhooks functionality on platforms without native webhooks support. Developers can receive real-time notifications of events from supported apps. Powered by Convoy.',
	ogImage: 'https://nohooks.io/seo-img/og-image.png',
	twitterImage: 'https://nohooks.io/seo-img/og-image.png',
	twitterCard: 'summary_large_image',
	twitterImageAlt: 'Nohooks description image',
	applicationName: 'Nohooks',
	twitterSite: '@getconvoy',
	twitterCreator: '@getconvoy',
	author: 'Convoy',
	creator: 'Convoy',
	ogUrl: 'https://nohooks.io'
});
</script>
<style lang="scss">
html {
	@apply scroll-smooth;
}
</style>
