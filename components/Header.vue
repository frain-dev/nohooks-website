<template>
	<header>
		<nav class="w-full mx-auto bg-white-100 z-50 fixed left-[50%] -translate-x-1/2 translate-y-0 transition-all duration-300 shadow-[inset_0px_-3px_8px_rgba(255,255,255,0.07)] backdrop-blur-[36]">
			<div class="flex items-center max-w-[1044px] mx-auto px-20px pt-20px">
				<div class="flex items-center">
					<button class="mr-26px hidden desktop:block" @click="showMenu = !showMenu">
						<img src="/svg/menu-icon.svg" alt="menu icon" :class="`w-20px transition-all duration-300 ${showMenu ? 'rotate-90' : ''}`" />
					</button>
					<NuxtLink to="/">
						<img src="/svg/logo.svg" alt="Nohooks logo" class="h-38px" />
					</NuxtLink>
				</div>

				<ul
					class="flex items-center gap-60px ml-62px desktop:ml-0 desktop:absolute desktop:top-90px desktop:left-20px desktop:min-w-[250px] desktop:bg-white-100 desktop:flex-col desktop:shadow-sm desktop:rounded-12px desktop:pl-24px desktop:py-14px transition-all duration-500"
					:class="showMenu ? 'desktop:h-fit desktop:block desktop:z-50' : 'desktop:hidden desktop:h-0'"
				>
					<li class="text-gray-600 text-16 desktop:py-10px desktop:border-b desktop:border-b-primary-25 desktop:last-of-type:border-none" v-for="(menu, i) in menuItems" :key="i">
						<NuxtLink v-if="menu.type == 'route'" :to="menu.route">{{ menu.link }}</NuxtLink>
						<NuxtLink v-else target="_blank" :to="menu.route">{{ menu.link }}</NuxtLink>
					</li>
				</ul>

				<ul class="ml-auto flex items-center gap-24px">
					<li>
						<NuxtLink target="_blank" to="https://github.com/frain-dev/convoy">
							<img src="/img/github.png" alt="github logo" />
						</NuxtLink>
					</li>
					<li>
						<NuxtLink target="_blank" to="https://app.nohooks.io" class="px-16px py-12px text-14 font-normal border border-primary-400 rounded-8px text-primary-400">Get Started</NuxtLink>
					</li>
				</ul>
			</div>
		</nav>

		<div class="fixed top-0 left-0 w-full h-full bg-black bg-opacity-10 backdrop-blur-[25px] transition-all duration-500" :class="showMenu ? 'pointer-events-all opacity-100 z-[2]' : 'pointer-events-none opacity-0'" @click="showMenu = !showMenu"></div>
	</header>
</template>
<script setup lang="ts">
const showMenu = ref(false);

const menuItems = [
	{ link: 'Pricing', route: '/#pricing', type: 'route' },
	{ link: 'Features', route: '/#features', type: 'route' },
	{ link: 'Docs', route: 'https://sincere-braid-52e.notion.site/Nohooks-Documentation-4125058d7991424a86342d0ee245165f', type: 'url' },
	{ link: 'Blog', route: 'https://getconvoy.io/blog', type: 'url' }
];
</script>
