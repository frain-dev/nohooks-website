<template>
    <div>

        <header>
            <nav class="flex items-center justify-between max-w-[900px] mx-auto p-20px">
                <NuxtLink to="/" class="logo">
                    <h1 class="font-bold text-gray-600 text-16">Nohooks</h1>
                </NuxtLink>

                <ul class="flex items-center justify-between gap-24px">
                    <li>
                        <NuxtLink to="https://github.com/frain-dev/unoffical-webhooks">
                            <img src="~/assets/img/github.png" alt="github logo">
                        </NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="https://app.nohooks.io" class="px-10px py-8px text-14 font-normal bg-primary-25 rounded-8px text-primary-400">Login / Sign up</NuxtLink>
                    </li>
                </ul>
            </nav>
        </header>

        <main class="pb-200px">
            <section class="max-w-[900px] mx-auto p-20px py-110px text-center flex flex-col gap-50px items-center">
                <h1 class="text-[48px] font-bold leading-[60px] bg-clip-text">Webhooks on Platforms with Nohooks</h1>
                <p class="text-gray-500 text-16 max-w-[500px]">Nohooks enables you to connect and start receiving webhook events based on activities from third party platforms like Notion and Render, with more platforms coming soon.</p>


                <div class="flex items-center gap-24px justify-center flex-wrap mx-auto w-fit">
                    <NuxtLink to="https://app.nohooks.io" target="_blank" id="cta-button" class="flex items-center py-12px px-16px gap-26px w-fit text-white-100 rounded-8px shadow-xl hover:shadow-2xl transition-all duration-300 cursor-pointer">
                        Connect Your Account
                        <svg width="15" height="14" viewBox="0 0 15 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M7.56635 8.97749L5.30302 11.2408C5.16915 11.3752 5.01006 11.4819 4.83488 11.5546C4.6597 11.6274 4.47187 11.6648 4.28218 11.6648C4.09249 11.6648 3.90467 11.6274 3.72949 11.5546C3.55431 11.4819 3.39522 11.3752 3.26135 11.2408C3.12625 11.1073 3.01899 10.9484 2.94578 10.7732C2.87257 10.5979 2.83488 10.4099 2.83488 10.22C2.83488 10.0301 2.87257 9.84205 2.94578 9.66682C3.01899 9.49158 3.12625 9.33262 3.26135 9.19915L5.52468 6.93582C5.63453 6.82598 5.69624 6.677 5.69624 6.52165C5.69624 6.36631 5.63453 6.21733 5.52468 6.10749C5.41484 5.99764 5.26586 5.93593 5.11052 5.93593C4.95517 5.93593 4.80619 5.99764 4.69635 6.10749L2.43302 8.37665C1.97706 8.87295 1.73046 9.52621 1.74473 10.2C1.75899 10.8738 2.03301 11.516 2.50957 11.9926C2.98612 12.4692 3.62836 12.7432 4.30216 12.7574C4.97596 12.7717 5.62922 12.5251 6.12552 12.0692L8.39468 9.80582C8.50453 9.69598 8.56624 9.547 8.56624 9.39165C8.56624 9.23631 8.50453 9.08733 8.39468 8.97749C8.28484 8.86764 8.13586 8.80593 7.98052 8.80593C7.82517 8.80593 7.67619 8.86764 7.56635 8.97749V8.97749ZM5.65302 8.84915C5.70752 8.90322 5.77217 8.94599 5.84324 8.97502C5.91431 9.00405 5.99041 9.01876 6.06718 9.01832C6.14395 9.01876 6.22006 9.00405 6.29113 8.97502C6.3622 8.94599 6.42684 8.90322 6.48135 8.84915L9.35135 5.97915C9.46119 5.86931 9.5229 5.72033 9.5229 5.56499C9.5229 5.40964 9.46119 5.26066 9.35135 5.15082C9.24151 5.04098 9.09253 4.97927 8.93718 4.97927C8.78184 4.97927 8.63286 5.04098 8.52302 5.15082L5.65302 8.02082C5.59834 8.07505 5.55494 8.13957 5.52533 8.21065C5.49571 8.28173 5.48047 8.35798 5.48047 8.43499C5.48047 8.51199 5.49571 8.58824 5.52533 8.65932C5.55494 8.73041 5.59834 8.79492 5.65302 8.84915ZM12.7522 10.5H12.1688V9.91665C12.1688 9.76194 12.1074 9.61357 11.998 9.50417C11.8886 9.39478 11.7402 9.33332 11.5855 9.33332C11.4308 9.33332 11.2824 9.39478 11.173 9.50417C11.0636 9.61357 11.0022 9.76194 11.0022 9.91665V10.5H10.4188C10.2641 10.5 10.1158 10.5614 10.0064 10.6708C9.89697 10.7802 9.83552 10.9286 9.83552 11.0833C9.83552 11.238 9.89697 11.3864 10.0064 11.4958C10.1158 11.6052 10.2641 11.6667 10.4188 11.6667H11.0022V12.25C11.0022 12.4047 11.0636 12.5531 11.173 12.6625C11.2824 12.7719 11.4308 12.8333 11.5855 12.8333C11.7402 12.8333 11.8886 12.7719 11.998 12.6625C12.1074 12.5531 12.1688 12.4047 12.1688 12.25V11.6667H12.7522C12.9069 11.6667 13.0553 11.6052 13.1647 11.4958C13.2741 11.3864 13.3355 11.238 13.3355 11.0833C13.3355 10.9286 13.2741 10.7802 13.1647 10.6708C13.0553 10.5614 12.9069 10.5 12.7522 10.5ZM10.308 7.89249L12.5713 5.62332C13.0273 5.12702 13.2739 4.47376 13.2596 3.79996C13.2454 3.12616 12.9714 2.48393 12.4948 2.00737C12.0182 1.53082 11.376 1.25679 10.7022 1.24253C10.0284 1.22826 9.37515 1.47486 8.87885 1.93082L6.60968 4.19415C6.55529 4.24854 6.51215 4.31311 6.48272 4.38417C6.45328 4.45524 6.43813 4.5314 6.43813 4.60832C6.43813 4.68524 6.45328 4.7614 6.48272 4.83246C6.51215 4.90353 6.55529 4.9681 6.60968 5.02249C6.66407 5.07687 6.72864 5.12002 6.7997 5.14945C6.87077 5.17889 6.94693 5.19404 7.02385 5.19404C7.10077 5.19404 7.17693 5.17889 7.248 5.14945C7.31906 5.12002 7.38363 5.07687 7.43802 5.02249L9.70135 2.75915C9.83522 2.62476 9.99431 2.51812 10.1695 2.44535C10.3447 2.37259 10.5325 2.33513 10.7222 2.33513C10.9119 2.33513 11.0997 2.37259 11.2749 2.44535C11.4501 2.51812 11.6091 2.62476 11.743 2.75915C11.8781 2.89262 11.9854 3.05158 12.0586 3.22682C12.1318 3.40205 12.1695 3.59007 12.1695 3.77999C12.1695 3.9699 12.1318 4.15792 12.0586 4.33315C11.9854 4.50839 11.8781 4.66735 11.743 4.80082L9.47968 7.06415C9.42501 7.11838 9.38161 7.1829 9.352 7.25398C9.32238 7.32507 9.30713 7.40131 9.30713 7.47832C9.30713 7.55533 9.32238 7.63157 9.352 7.70266C9.38161 7.77374 9.42501 7.83826 9.47968 7.89249C9.53391 7.94716 9.59843 7.99056 9.66951 8.02017C9.7406 8.04979 9.81684 8.06503 9.89385 8.06503C9.97086 8.06503 10.0471 8.04979 10.1182 8.02017C10.1893 7.99056 10.2538 7.94716 10.308 7.89249V7.89249Z"
                                fill="#EDF2F7" />
                        </svg>
                    </NuxtLink>
                    <NuxtLink to="/" target="_blank" class="flex items-center py-12px px-16px w-fit text-primary-400 border border-primary-400 rounded-8px cursor-pointer">Documentation</NuxtLink>
                </div>

                <NuxtLink to="https://getconvoy.io/cloud" class="text-14 text-gray-500 font-normal">Powered by <span class="text-primary-400">Convoy</span></NuxtLink>
            </section>

            <section class="px-20px max-w-[988px] w-full mx-auto bg-[url(~/assets/img/video-screenshot.png)] bg-contain bg-center bg-no-repeat">
                <video loop autoplay class="rounded-24px shadow-sm border border-primary-50 w-full min-h-[500px]">
                    <source src="~/assets/videos/demo.mp4" type="video/mp4" />
                    <p>
                        Your browser doesn't support HTML video. Here is a
                        <a href="~/assets/videos/demo.mp4">link to the video</a> instead.
                    </p>
                    <img src="~/assets/img/video-screenshot.png" class="shadow-sm border border-primary-50 w-full min-h-[500px]" alt="video screenshot">
                </video>
            </section>
        </main>

        <p class="text-12 text-center text-gray-400 pb-50px">© 2023 Frain Technologies Inc</p>
    </div>
</template>

<style lang="scss">
section {
    h1 {
        background: linear-gradient(182deg, rgb(29 41 57 / 0%), rgba(71, 125, 179, 1), rgb(29 41 57 / 72%));
        -webkit-background-clip: text;
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    #cta-button {
        background: linear-gradient(180deg, rgb(71 125 179 / 56%) 0%, #477DB3 95.83%, #477DB3 100%);

    }
}
</style>