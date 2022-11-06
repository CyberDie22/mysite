<script lang="ts">
    import "../app.css";

    function switchRoute(route: string) {
        return () => { window.location.assign(window.origin + route) }
    }
</script>

<div class="flex items-center justify-center h-screen w-screen">
    <div class="md:container md:mx-10 md:rounded-xl grid w-screen h-[calc(100vh*0.75)] bg-gray-900" style="grid-template-rows: 50px 100%">
        <div class="md:rounded-t-xl bg-white bg-opacity-5 grid grid-cols-7 gap-5 px-5 text-center">
            <!-- svelte-ignore a11y-click-events-have-key-events -->
            <div class="md:rounded-tl-xl transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer" on:click|stopPropagation={switchRoute("/")}>Home</div>
            <!-- svelte-ignore a11y-click-events-have-key-events -->
            <div class="transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer" on:click|stopPropagation={switchRoute("/skills")}>Skills</div>
            <!-- <div class="transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer"></div> -->
            <!-- <div class="transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer"></div> -->
            <!-- <div class="transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer"></div> -->
            <!-- <div class="transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer"></div> -->
            <!-- <div class="transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer"></div> -->
            <!-- <div class="md:rounded-tr-xl transition ease-in-out py-3 hover:bg-black hover:bg-opacity-5 hover:cursor-pointer"></div> -->
        </div>

        <div class="p-5">
            <slot />
        </div>
    </div>
</div>