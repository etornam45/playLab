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
        width="400"
    />
    <img
        class="absolute top-[80%] right-0 hover:right-[20px] translate-x-[-50%] translate-y-[-50%]"
        src="/Knife_ill.png"
        alt=""
        width="150"
    />
</section>

<style>
    .hero_art {
        background-image: url("/Hero_Art.png");
        background-size: contain !important;
        cursor: pointer;
    }

    .hero_art:hover:before {
        content: "";
        position: absolute;
        top: 0;
        width: 100%;
        height: 100%;
        background: inherit;
        filter: blur(50px) saturate(5) drop-shadow(0 0 10px #68FF04);
        z-index: -10;
        
    }
</style>
