<script lang="ts">
    import gsrcLabImg from '$lib/assets/images/gsrc_research_lab.jpg';
    import snipImg from '$lib/assets/images/gsrc.jpg';
    import ggcmpImg from '$lib/assets/images/ggcmp.jpg';
    import DocsPreview from '$lib/components/DocsPreview/DocsPreview.svelte';

    // Components
    import { ListBox, ListBoxItem } from '@skeletonlabs/skeleton';

    // Local
    let showcase = 'GGCMP';
</script>

<div class="grid grid-cols-1 lg:grid-cols-3 gap-4 md:gap-10 items-start">
    <!-- Preview -->
    <div class="col-span-2">
        <DocsPreview label={showcase.replace('-', ' ')} regionPreview="min-h-[400px]">
            <svelte:fragment slot="preview">
                {#if showcase === 'GGCMP'}
                    <div class="card shadow-xl overflow-hidden max-w-[400px] text-token">
                        <header>
                            <img
                                src={ggcmpImg}
                                class="bg-black/50 w-full h-1/2 aspect-[21/9] object-cover"
                                alt="Svelsa"
                                loading="lazy"
                            />
                        </header>
                        <div class="p-4 space-y-4">
                            <p class="h6 font-bold">Mineral Analysis</p>
                            <h3 class="h3">Gujarat Geo-Chemical Mapping Project (GGCMP)</h3>
                            <article>
                                <p class="opacity-75">
                                    Contributed to the Gujarat Geo-Chemical Mapping Project by
                                    performing laboratory-based elemental analysis of soil and
                                    sediment samples using XRF, AAS, and wet chemistry methods.
                                </p>
                            </article>
                        </div>
                        <hr class="opacity-50" />
                        <footer class="p-4 flex justify-center items-center space-x-4">
                            <div class="flex justify-center space-x-2">
                                <a
                                    href="https://gmrds.gujarat.gov.in/"
                                    class="group chip variant-soft hover:variant-filled"
                                    aria-label="GMRDS Link"
                                >
                                    <svg
                                        xmlns="http://www.w3.org/2000/svg"
                                        height="1.5em"
                                        viewBox="0 0 512 512"
                                    >
                                        <path
                                            class="fill-black dark:fill-white group-hover:fill-white group-hover:dark:fill-black"
                                            d="M352 256c0 22.2-1.2 43.6-3.3 64l-185.3 0c-2.2-20.4-3.3-41.8-3.3-64s1.2-43.6 3.3-64l185.3 0c2.2 20.4 3.3 41.8 3.3 64zm28.8-64l123.1 0c5.3 20.5 8.1 41.9 8.1 64s-2.8 43.5-8.1 64l-123.1 0c2.1-20.6 3.2-42 3.2-64s-1.1-43.4-3.2-64zm112.6-32l-116.7 0c-10-63.9-29.8-117.4-55.3-151.6c78.3 20.7 142 77.5 171.9 151.6zm-149.1 0l-176.6 0c6.1-36.4 15.5-68.6 27-94.7c10.5-23.6 22.2-40.7 33.5-51.5C239.4 3.2 248.7 0 256 0s16.6 3.2 27.8 13.8c11.3 10.8 23 27.9 33.5 51.5c11.6 26 20.9 58.2 27 94.7zm-209 0L18.6 160C48.6 85.9 112.2 29.1 190.6 8.4C165.1 42.6 145.3 96.1 135.3 160zM8.1 192l123.1 0c-2.1 20.6-3.2 42-3.2 64s1.1 43.4 3.2 64L8.1 320C2.8 299.5 0 278.1 0 256s2.8-43.5 8.1-64zM194.7 446.6c-11.6-26-20.9-58.2-27-94.6l176.6 0c-6.1 36.4-15.5 68.6-27 94.6c-10.5 23.6-22.2 40.7-33.5 51.5C272.6 508.8 263.3 512 256 512s-16.6-3.2-27.8-13.8c-11.3-10.8-23-27.9-33.5-51.5zM135.3 352c10 63.9 29.8 117.4 55.3 151.6C112.2 482.9 48.6 426.1 18.6 352l116.7 0zm358.1 0c-30 74.1-93.6 130.9-171.9 151.6c25.5-34.2 45.2-87.7 55.3-151.6l116.7 0z"
                                        />
                                    </svg>
                                    <span>Website</span>
                                </a>
                            </div>
                        </footer>
                    </div>
                {:else if showcase === "GSRC's-Project"}
                    <div class="card shadow-xl overflow-hidden max-w-[400px] text-token">
                        <header>
                            <img
                                src={snipImg}
                                class="bg-black/50 w-full h-1/2 aspect-[21/9] object-cover"
                                alt="GSRC"
                                loading="lazy"
                            />
                        </header>
                        <div class="p-4 space-y-4">
                            <p class="h6 font-bold">R & D</p>
                            <h3 class="h3">GSRC: Development of coal and lignite additives</h3>
                            <article>
                                <p class="opacity-75">
                                    Currently engaged in the development of functional additives for
                                    coal and lignite to enhance combustion efficiency, elevate
                                    calorific value, and mitigate emissions of NOₓ, SOₓ, and
                                    particulate matter. This research aims to advance cleaner
                                    combustion technologies and is being evaluated through
                                    controlled laboratory-scale experiments.
                                </p>
                            </article>
                        </div>
                        <hr class="opacity-50" />
                        <footer class="p-4 flex justify-center items-center space-x-4">
                            <div class="flex justify-center space-x-2">
                                <a
                                    href="https://gsrc.res.in/research-and-development/"
                                    class="group chip variant-soft hover:variant-filled"
                                    aria-label="GSRC Link"
                                >
                                    <svg
                                        xmlns="http://www.w3.org/2000/svg"
                                        height="1.5em"
                                        viewBox="0 0 512 512"
                                    >
                                        <path
                                            class="fill-black dark:fill-white group-hover:fill-white group-hover:dark:fill-black"
                                            d="M352 256c0 22.2-1.2 43.6-3.3 64l-185.3 0c-2.2-20.4-3.3-41.8-3.3-64s1.2-43.6 3.3-64l185.3 0c2.2 20.4 3.3 41.8 3.3 64zm28.8-64l123.1 0c5.3 20.5 8.1 41.9 8.1 64s-2.8 43.5-8.1 64l-123.1 0c2.1-20.6 3.2-42 3.2-64s-1.1-43.4-3.2-64zm112.6-32l-116.7 0c-10-63.9-29.8-117.4-55.3-151.6c78.3 20.7 142 77.5 171.9 151.6zm-149.1 0l-176.6 0c6.1-36.4 15.5-68.6 27-94.7c10.5-23.6 22.2-40.7 33.5-51.5C239.4 3.2 248.7 0 256 0s16.6 3.2 27.8 13.8c11.3 10.8 23 27.9 33.5 51.5c11.6 26 20.9 58.2 27 94.7zm-209 0L18.6 160C48.6 85.9 112.2 29.1 190.6 8.4C165.1 42.6 145.3 96.1 135.3 160zM8.1 192l123.1 0c-2.1 20.6-3.2 42-3.2 64s1.1 43.4 3.2 64L8.1 320C2.8 299.5 0 278.1 0 256s2.8-43.5 8.1-64zM194.7 446.6c-11.6-26-20.9-58.2-27-94.6l176.6 0c-6.1 36.4-15.5 68.6-27 94.6c-10.5 23.6-22.2 40.7-33.5 51.5C272.6 508.8 263.3 512 256 512s-16.6-3.2-27.8-13.8c-11.3-10.8-23-27.9-33.5-51.5zM135.3 352c10 63.9 29.8 117.4 55.3 151.6C112.2 482.9 48.6 426.1 18.6 352l116.7 0zm358.1 0c-30 74.1-93.6 130.9-171.9 151.6c25.5-34.2 45.2-87.7 55.3-151.6l116.7 0z"
                                        />
                                    </svg>
                                    <span>Website</span>
                                </a>
                            </div>
                        </footer>
                    </div>
                {:else if showcase === 'GSRC-Laboratory'}
                    <div class="card shadow-xl overflow-hidden max-w-[400px] text-token">
                        <header>
                            <img
                                src={gsrcLabImg}
                                class="bg-black/50 w-full h-1/2 aspect-[21/9] object-cover"
                                alt="Post"
                                loading="lazy"
                            />
                        </header>
                        <div class="p-4 space-y-4">
                            <p class="h6 font-bold">Analysis</p>
                            <h3 class="h3">
                                GSRC: Development of Laboratory for Critical Metals including REEs
                            </h3>
                            <article>
                                <p class="opacity-75">
                                    Establishing a specialized laboratory for the identification,
                                    characterization, and analysis of critical metals, with a focus
                                    on Rare Earth Elements (REEs). The lab aims to support advanced
                                    separation techniques, improve analytical precision, and
                                    contribute to sustainable and efficient resource utilization.
                                </p>
                            </article>
                        </div>
                        <hr class="opacity-50" />
                        <footer class="p-4 flex justify-center items-center space-x-4">
                            <div class="flex justify-center space-x-2">
                                <a
                                    href="https://gsrc.res.in/research-and-development/"
                                    class="group chip variant-soft hover:variant-filled"
                                    aria-label="GSRC Link"
                                >
                                    <svg
                                        xmlns="http://www.w3.org/2000/svg"
                                        height="1.5em"
                                        viewBox="0 0 512 512"
                                    >
                                        <path
                                            class="fill-black dark:fill-white group-hover:fill-white group-hover:dark:fill-black"
                                            d="M352 256c0 22.2-1.2 43.6-3.3 64l-185.3 0c-2.2-20.4-3.3-41.8-3.3-64s1.2-43.6 3.3-64l185.3 0c2.2 20.4 3.3 41.8 3.3 64zm28.8-64l123.1 0c5.3 20.5 8.1 41.9 8.1 64s-2.8 43.5-8.1 64l-123.1 0c2.1-20.6 3.2-42 3.2-64s-1.1-43.4-3.2-64zm112.6-32l-116.7 0c-10-63.9-29.8-117.4-55.3-151.6c78.3 20.7 142 77.5 171.9 151.6zm-149.1 0l-176.6 0c6.1-36.4 15.5-68.6 27-94.7c10.5-23.6 22.2-40.7 33.5-51.5C239.4 3.2 248.7 0 256 0s16.6 3.2 27.8 13.8c11.3 10.8 23 27.9 33.5 51.5c11.6 26 20.9 58.2 27 94.7zm-209 0L18.6 160C48.6 85.9 112.2 29.1 190.6 8.4C165.1 42.6 145.3 96.1 135.3 160zM8.1 192l123.1 0c-2.1 20.6-3.2 42-3.2 64s1.1 43.4 3.2 64L8.1 320C2.8 299.5 0 278.1 0 256s2.8-43.5 8.1-64zM194.7 446.6c-11.6-26-20.9-58.2-27-94.6l176.6 0c-6.1 36.4-15.5 68.6-27 94.6c-10.5 23.6-22.2 40.7-33.5 51.5C272.6 508.8 263.3 512 256 512s-16.6-3.2-27.8-13.8c-11.3-10.8-23-27.9-33.5-51.5zM135.3 352c10 63.9 29.8 117.4 55.3 151.6C112.2 482.9 48.6 426.1 18.6 352l116.7 0zm358.1 0c-30 74.1-93.6 130.9-171.9 151.6c25.5-34.2 45.2-87.7 55.3-151.6l116.7 0z"
                                        />
                                    </svg>
                                    <span>Website</span>
                                </a>
                            </div>
                        </footer>
                    </div>
                {/if}
            </svelte:fragment>
        </DocsPreview>
    </div>
    <!-- Info -->
    <div class="space-y-4" id="My_Projects">
        <h2 class="h2">My Projects!</h2>
        <p>
            Science is built on trial, error, and revision this portfolio is no exception. If
            something seems off, it might just be a hypothesis waiting for your peer review.
        </p>
        <!-- Options -->
        <ListBox
            active="variant-filled"
            hover="hover:variant-soft"
            rounded="rounded-container-token"
            padding="!p-4"
            labelledby="My_Projects"
        >
            <ListBoxItem bind:group={showcase} name="showcase" value="GGCMP">
                <div class="space-y-2">
                    <h3 class="h3">GGCMP: Gujarat Geo-Chemical Mapping Project</h3>
                    <p class="!text-sm">
                        The GGCMP aims to establish a geochemical baseline for Gujarat to support
                        mineral exploration, environmental assessment, and sustainable land-use
                        planning.
                    </p>
                </div>
            </ListBoxItem>
            <ListBoxItem bind:group={showcase} name="showcase" value="GSRC's-Project">
                <div class="space-y-2">
                    <h3 class="h3">GSRC: Development of coal and lignite additives</h3>
                    <p class="!text-sm">
                        Studying coal and lignite additives to improve combustion efficiency,
                        enhance calorific value, and reduce emissions through lab-scale testing.
                    </p>
                </div>
            </ListBoxItem>
            <ListBoxItem bind:group={showcase} name="showcase" value="GSRC-Laboratory">
                <div class="space-y-2">
                    <h3 class="h3">
                        GSRC: Development of Laboratory for Critical Metals including REEs
                    </h3>
                    <p class="!text-sm">
                        Developing a specialized laboratory for accurate identification and analysis
                        of critical metals, focusing on rare earth elements (REEs) to support
                        sustainable resource development.
                    </p>
                </div>
            </ListBoxItem>
            <!-- <ListBoxItem
                bind:group={showcase}
                name="showcase"
                value="link"
                on:click={() => {
                    window.location.href = 'https://github.com/Hetarth02';
                }}
            >
                <div class="space-y-2">
                    <h3 class="h3">🔭And many more...</h3>
                    <p class="!text-sm">There is much more to explore!</p>
                </div>
            </ListBoxItem> -->
        </ListBox>
    </div>
</div>
