<script>
    export let y;
    let tabs =[
        {name:"Projects", link: '#projects'},
        {name:"About Me", link: '#about'}
    ]

</script>

<header class={'sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border border-solid '+ (
    y > 0 ? 'pt-4 bg-slate-950 border-violet-950': 'py-6 bg-transparent border-transparent'
)}>
    <a href="#">
    <h1 class="font-medium">
        <b class="font-bold Reddit-Mono">Sudhamshu</b> Suri
    </h1>
    </a>
    <div class="sm:flex items-center gap-4 hidden">
        {#each tabs as tab, index}
        <a href={tab.link} class="duration-200 hover:text-violet-400">
            <p>{tab.name}</p>
        </a>
        {/each}
    </div>
    <a href="https://github.com/SudhamshuSuri" target="_blank" class="blueShadow relative float overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950">
        <div class="absolute top-0 right-full w-full h-full bg-violet opacity-20 group-hover:translatex-full z-0 duration 200" />
        <h4 class="relative z-9">Get in Touch!</h4>
    </a>
</header>