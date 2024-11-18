<script>
    import GameCard from "$lib/components/GameCard.svelte";

</script>
<main class="h-[10000px] bg-yellow-500 grid-view">
    <header
        class="sticky top-2 flex w-full justify-between items-center max-container p-2 shadow text-xl z-10 bg-yellow-400/50 backdrop-blur-md"
    >
        <h1 class="font-black ml-4 text-[#68FF04] text-shadow">PlayLab</h1>

        <nav
            class="flex gap-4 text-xl font-extrabold text-[blueviolet] text-shadow"
        >
            <a href="#">All Games</a>
            <a href="#">New Games</a>
            <a href="#">Action</a>
            <a href="#">Adventure</a>
            <a href="#">Sports</a>
        </nav>

        <form>
            <input class="p-2 shadow" type="text" placeholder="Search" />
            <button class="p-2 px-4 bg-green-400 shadow">Search</button>
        </form>
    </header>

    <section class="relative min-h-screen w-full">
        <div
            class="hero_art absolute w-[1000px] h-[700px] bg-cover bg-no-repeat top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%]"
            style="background-image: url('/Hero_Art.png');"
        >
            <img
                class="absolute still top-0 left-0 translate-x-[-50%] translate-y-[-50%] w-full h-full"
                src="/Hero_Art.png"
                alt=""
            />
        </div>
        <img
            class="absolute breathe top-[20%] left-[50px] hover:left-[100px] translate-x-[-50%] translate-y-[-50%]"
            src="/Console_ill.png"
            alt=""
            width="150"
        />
        <img
            class="absolute top-[20%] right-0 hover:right-[20px] translate-x-[-50%] translate-y-[-50%] breathe"
            src="/football.png"
            alt=""
            width="150"
        />
        <img
            class="absolute top-[80%] left-[0px] hover:left-[50px] translate-x-[-50%] translate-y-[-50%]"
            src="/VR_ill.png"
            alt=""
            width="200"
        />
        <img
            class="absolute top-[80%] right-0 hover:right-[20px] translate-x-[-50%] translate-y-[-50%]"
            src="/Knife_ill.png"
            alt=""
            width="150"
        />
    </section>

    <section class="max-container">
        <h2 class="p-4 px-6 text-2xl font-black bg-white w-max shadow">Most Popular Games</h2>

        <div class="grid grid-cols-3 gap-8 mt-[100px]">
            <GameCard />
            <GameCard />
            <GameCard />
            <GameCard />
            <GameCard />
            <GameCard />
        </div>
    </section>

    <section>
        
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

    .hero_art {
        background-image: url("/Hero_Art.png");
        background-size: contain !important;
    }

    .hero_art::before {
        content: "";
        position: absolute;
        top: 0;
        width: 100%;
        height: 100%;
        background: inherit;
        filter: blur(100px) saturate(5);
        z-index: -10;
    }
</style>
