<script>
    import HeroSection from "$lib/components/HeroSection.svelte";
    import MostPopularSection from "$lib/components/MostPopularSection.svelte";
</script>

<main class=" bg-yellow-500 grid-view pb-[100px]">
    <header
        class="sticky top-2 flex w-full justify-between items-center max-container p-2 shadow text-xl z-10 bg-yellow-400/50 backdrop-blur-md backdrop-saturate-[10]"
    >
        <h1 class="font-black ml-4 text-[#68FF04] text-shadow">PlayLab</h1>

        <nav
            class="flex gap-4 text-xl font-extrabold text-[blueviolet]"
        >
            <a class="hover:scale-[1.1]" href="#">All Games</a>
            <a class="hover:scale-[1.1]" href="#">New Games</a>
            <a class="hover:scale-[1.1]" href="#">Action</a>
            <a class="hover:scale-[1.1]" href="#">Adventure</a>
            <a class="hover:scale-[1.1]" href="#">Sports</a>
        </nav>

        <form>
            <input class="p-2 shadow" type="text" placeholder="Search here" />
            <button class="p-2 px-4 bg-[#68FF04] shadow">Search</button>
        </form>
    </header>

    <HeroSection />

    <MostPopularSection />

    <section class="max-container mt-[100px]">
        <div>
            <a href="https://www.google.com" class="text-9xl font-mono font-black text-shadow hover:big-text-shadow cursor-alias hover:text-[#68FF04]">Play your favourite game at anytime</a>
            <p
                class="text-4xl  mt-8"
            >
                Subscribe to play your favourite games at anytime. <br> No need to <span class="bg-[#bc04ff] shadow px-2 text-white hover:big-shadow cursor-pointer">download</span> or install. Just join, play and enjoy.
            </p>
            <button class="bg-[#68FF04] p-4 px-8 mt-28 text-2xl font-bold text-shadow hover:big-shadow shadow">Subscribe Now</button>
            
        </div>
    </section>
</main>

<style>
    .grid-view {
        --size: 70px;
        --width: 4px;
        --color: rgba(243, 234, 234, 0.232);
        background-size: var(--size) var(--size);
        background-image: linear-gradient(
                to right,
                var(--color) var(--width),
                transparent var(--width)
            ),
            linear-gradient(
                to bottom,
                var(--color) var(--width),
                transparent var(--width)
            );
    }
</style>
