<template>
	<div class="bg-white-100">
		<Header></Header>
		<main class="pt-86px @container">
			<section
				class="max-w-[1210px] mx-auto px-16px pt-100px text-center flex flex-col items-center @[1280px]:bg-[url(/img/top-arrow.png)] @[1100px]:bg-[url(/img/top-arrow-md.png)] @[768px]:bg-[url(/img/top-arrow-sm.png)] bg-no-repeat @[1280px]:bg-[0.5%_0%] @[1220px]:bg-[1%_0%] @[1100px]:bg-[3%_0%] @[768px]:bg-[3.5%_0%] @[1280px]:bg-[length:22%] @[1100px]:bg-[length:10%] @[768px]:bg-[length:3.5%] mobile:bg-none"
			>
				<h1 class="text-gray-strong text-[60px] leading-[72px] desktop:text-[48px] desktop:leading-[62px] font-bold max-w-[718px]">Webhooks on Platforms Without Webhooks</h1>
				<p class="text-gray-normal text-16 mt-24px font-normal max-w-[718px]">Nohooks enables you to connect and start receiving webhook from third party platforms like Notion, Digital Ocean, and Render, with more platforms coming soon.</p>
			</section>

			<section class="relative overflow-hidden before:absolute before:top-0 before:left-0 before:w-full before:h-full before:animate-pulsate radial-bg before:-z-20 pt-40px">
				<div class="max-w-[1342px] mx-auto">
					<div
						class="flex flex-col items-center !bg-transparent @[1280px]:bg-[url(/img/bottom-arrow.png)] @[1000px]:bg-[url(/img/bottom-arrow-md.png)] @[840px]:bg-[url(/img/bottom-arrow-sm.png)] desktop:bg-none bg-no-repeat @[1280px]:bg-[87%_3.5%] @[1000px]:bg-[59px_1.5%] @[840px]:bg-[21px_1.5%] @[1280px]:bg-[length:85%] @[840px]:bg-[length:100%] px-16px"
					>
						<div class="flex items-center gap-26px mb-40px">
							<NuxtLink target="_blank" to="https://app.nohooks.io" class="rounded-8px px-16px py-12px border border-primary-400 bg-primary-400 text-14 text-gray-25">Get Started</NuxtLink>
							<NuxtLink to="https://github.com/frain-dev/nohooks-backend" target="_blank" class="rounded-8px px-16px py-12px border border-success-400 text-14 text-success-400">Star on Github</NuxtLink>
						</div>

						<div class="rounded-12px px-30px pt-30px desktop:px-24px desktop:pt-24px max-w-[820px] mx-auto bg-white-30 backdrop-blur-[21px] mb-54px">
							<img src="/img/HomePage.png" />
						</div>

						<p class="mb-32px text-gray-normal text-16">Supported Platforms</p>
						<ul class="flex items-center gap-50px">
							<li>
								<NuxtLink to="https://render.com/" target="_blank">
									<picture>
										<source srcset="/svg/render-dark.svg" media="(prefers-color-scheme:dark)" />
										<img src="/svg/render.svg" alt="render icon" />
									</picture>
								</NuxtLink>
							</li>
							<li>
								<NuxtLink to="https://www.notion.so/" target="_blank">
									<picture>
										<source srcset="/svg/Notion-dark.svg" media="(prefers-color-scheme:dark)" />
										<img src="/svg/Notion.svg" alt="notion icon" />
									</picture>
								</NuxtLink>
							</li>
							<li>
								<NuxtLink to="https://www.digitalocean.com/" target="_blank">
									<picture>
										<source srcset="/svg/digitalOcean-dark.svg" media="(prefers-color-scheme:dark)" />
										<img src="/svg/digitalOcean.svg" alt="digital ocean icon" />
									</picture>
								</NuxtLink>
							</li>
						</ul>

						<div class="flex flex-col items-center py-200px" id="features">
							<h3 class="text-gray-strong text-center text-28 lg:text-[32px] lg:leading-[52px] font-bold max-w-[520px] mx-auto">
								Everything You Need To Receive
								<span class="text-primary-400">Webhook</span>
								Events
							</h3>

							<div class="flex flex-wrap mt-50px gap-y-40px gap-x-70px desktop:gap-x-20px mobile:gap-x-0 max-w-[766px] w-full mx-auto">
								<div class="min-w-[339px]" v-for="(feature, index) in features" :key="index">
									<div class="pl-26px bg-[linear-gradient(#91B1D1_40%,rgba(255,255,255,0)_0%)] bg-left bg-repeat-y bg-[length:1px_12px]">
										<p class="text-18 text-gray-normal font-semibold mb-10px">{{ feature.feature }}</p>
										<p class="text-14 text-gray-normal font-normal lg:max-w-[320px]">{{ feature.description }}</p>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</section>

			<section id="pricing" class="flex flex-col items-center mb-200px px-20px">
				<h3 class="text-gray-strong text-[32px] leading-[52px] text-center font-bold mb-10px">
					Affordable Pricing to
					<span class="text-primary-400">‘Webhookify’</span>
					your dependencies
				</h3>

				<div class="flex flex-wrap items-center justify-center text-gray-normal">
					<div class="mr-26px text-18 mb-14px text-center md:w-full">All plans include:</div>
					<span class="flex items-center mr-20px text-16 desktop:text-14 last-of-type:mr-0 mb-14px" v-for="(inclusion, i) in inclusions" :key="i">
						<svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="mr-6px">
							<path
								d="M10.09 14.58L7.27231 11.7623C7.07753 11.5675 6.76191 11.5669 6.56645 11.761L5.85606 12.4664C5.66011 12.661 5.65899 12.9776 5.85356 13.1735L5.85481 13.1748L9.73645 17.0564C9.93171 17.2517 10.2483 17.2517 10.4436 17.0564L19.7364 7.76352C19.9317 7.56825 19.9317 7.25167 19.7364 7.05641L19.0336 6.35352L19.0333 6.35372C18.8382 6.15854 18.5217 6.15845 18.3264 6.35352L10.09 14.58Z"
								fill="#47CD89"
							/>
						</svg>
						{{ inclusion }}
					</span>
				</div>

				<div class="flex flex-wrap justify-center gap-24px max-w-[1036px] w-full mx-auto">
					<div class="rounded-12px border-[0.5px] border-transparent border-gradient p-24px @[768px]:max-w-[308px] w-full mt-36px" :class="{ pro: i == 2 }" v-for="(plan, i) in plans" :key="i">
						<div class="min-h-[134px] mb-24px">
							<p class="text-gray-strong font-medium text-14">{{ plan.plan }}</p>
							<p class="text-12 text-gray-normal mb-24px min-h-[40px]">
								{{ plan.description }}
							</p>
							<p class="font-bold text-18 text-gray-normal mb-16px">${{ plan.price }}/month</p>
							<div class="line w-full h-[1px]"></div>
						</div>
						<div class="flex items-center text-12 text-gray-normal font-normal mb-16px" v-for="feature in plan.features" :key="feature">
							<svg width="17" height="16" viewBox="0 0 17 16" fill="none" xmlns="http://www.w3.org/2000/svg" class="mr-8px">
								<path
									d="M6.89332 9.71998L5.01486 7.84151C4.88501 7.71166 4.6746 7.71129 4.54429 7.84068L4.07069 8.31094C3.94006 8.44066 3.93931 8.65171 4.06903 8.78234L4.06986 8.78318L6.65762 11.3709C6.7878 11.5011 6.99885 11.5011 7.12903 11.3709L13.3243 5.17568C13.4545 5.0455 13.4545 4.83445 13.3243 4.70427L12.8557 4.23568L12.8556 4.23581C12.7254 4.10569 12.5145 4.10563 12.3843 4.23568L6.89332 9.71998Z"
									fill="#98A2B3"
								/>
							</svg>

							{{ feature }}
						</div>
						<NuxtLink target="_blank" to="https://app.nohooks.io" class="mt-24px block w-full text-gray-25 text-10 text-center font-medium rounded-8px p-10px" :class="i == 2 ? 'bg-success-400' : 'bg-primary-400'">
							{{ i == 0 ? 'Start for free' : 'Get Started' }}
						</NuxtLink>
					</div>
				</div>
			</section>

			<section class="flex flex-col items-center text-center mb-150px px-16px">
				<h3 class="text-gray-strong text-[32px] leading-[52px] font-bold max-w-[520px] mb-16px">
					We
					<span class="text-primary-400">Love</span>
					Open-Source
				</h3>

				<p class="text-16 text-gray-normal font-normal max-w-[592px] mb-40px">Source code powering Nohooks is available on Github. Forks, contributions, and reviews are welcomed.</p>

				<NuxtLink to="https://github.com/frain-dev/nohooks-backend" target="_blank" class="bg-gray-600 text-14 text-gray-25 py-12px px-16px rounded-8px flex items-center">
					<img src="/svg/github.svg" alt="github logo" class="h-16px w-16px mr-8px" />
					Star on Github
				</NuxtLink>
			</section>

			<section class="bg-white-100">
                <Footer></Footer>
            </section>
		</main>
	</div>
</template>
<script setup lang="ts">
const features = [
	{ feature: 'Failure Alerts', description: 'Get notified via email or slack about failed events and retries; as soon as they happen, you don’t have to worry about being blind sided.' },
	{ feature: 'Custom Endpoint Configuration', description: 'Endpoint configurations including endpoint authentication and timeout for each of your endpoints, no change is required on your existing endpoints.' },
	{ feature: 'Debuggable UI', description: 'Nohook’s friendly developer experience enables you to review and debug your webhook events. You have everything you need in view.' },
	{ feature: 'Automatic and Manual Retries', description: 'With retry configuration, you can be rest assured not to miss any beat of event sent to you in addition to manual retry; if needed.' }
];

const inclusions = ['Custom retry config', 'Enterprise level security', '30days data retention'];

const plans = [
	{ plan: 'Hobby', description: 'Free forever for hobby use', price: 0, features: ['3 Platform connections', '10,000 Events per connection', 'One user access', 'Unlimited endpoints per connection'] },
	{ plan: 'Mid', description: 'For average users needing to connect more platforms; with room for more event appetite', price: 20, features: ['6 Platform connections', '200,000 Events per connection ', '2 Team members limit', 'Unlimited endpoints per connection'] },
	{ plan: 'Pro', description: 'For pro users connecting multiple platforms and receiving even more events.', price: 50, features: ['Unlimited platform connections', '1million Events per connection ', 'Unlimited team members access', 'Unlimited endpoints per connection'] }
];
</script>
<style lang="scss">
.border-gradient {
	background: linear-gradient(var(--white-100), var(--white-100)) padding-box, linear-gradient(45deg, #a9efc500 10%, rgba(71, 125, 179, 1) 100%) border-box;

	&.pro {
		background: linear-gradient(var(--white-100), var(--white-100)) padding-box, linear-gradient(45deg, #dcfae600 10%, #17b26a 100%) border-box;

		.line {
			background: linear-gradient(15deg, #a9efc500 5%, #a9efc5 100%);
		}
	}
	.line {
		background: linear-gradient(15deg, #a9efc500 5%, #dae5f0 100%);
	}
}
</style>
