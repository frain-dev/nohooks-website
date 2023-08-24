<template>
	<footer>
		<div class="flex items-center mobile:items-start mobile:flex-col max-w-[1320px] px-20px mx-auto mb-80px">
			<div>
				<div class="flex items-center mb-12px">
					<NuxtLink to="https://app.nohooks.io" class="mr-12px">
						<img src="~/assets/svg/logo.svg" alt="Nohooks logo" class="h-38px" />
					</NuxtLink>
					<span class="text-primary-400 text-30 mobile:text-24 font-bold">Nohooks</span>
				</div>
				<NuxtLink to="https://getconvoy.io/" class="text-gray-600 text-10 font-normal">Powered By Convoy</NuxtLink>
			</div>

			<ul class="flex mobile:flex-col gap-60px md:gap-40px mobile:gap-24px ml-auto mobile:ml-[unset] mobile:mt-30px">
				<li class="text-16 text-gray-600" v-for="(link, i) in footerLinks" :key="i">
					<NuxtLink :to="link.route">{{ link.link }}</NuxtLink>
				</li>
			</ul>
		</div>
	</footer>
</template>
<script setup lang="ts">
const footerLinks = [
	{ link: 'Pricing', route: '/#pricing' },
	{ link: 'Features', route: '/#features' },
	{ link: 'Docs', route: 'https://sincere-braid-52e.notion.site/Nohooks-Documentation-4125058d7991424a86342d0ee245165f' },
	{ link: 'Blog', route: 'https://getconvoy.io/blog' },
	{ link: 'Github', route: 'https://github.com/frain-dev/convoy' },
	{ link: 'Convoy', route: 'https://getconvoy.io/' }
];
</script>
