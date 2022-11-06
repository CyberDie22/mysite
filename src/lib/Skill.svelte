<script lang="ts">
    function getIcon(name: string) {
        return `https://raw.githubusercontent.com/devicons/devicon/master/icons/${name}/${name}-original.svg`
    }
    function getPlainIcon(name: string) {
        return `https://raw.githubusercontent.com/devicons/devicon/master/icons/${name}/${name}-plain.svg`
    }

    function getIconFromProps() {
        if (isPlain) return getPlainIcon(name)
        else return getIcon(name)
    }

    function redirect() {
        window.location.assign(url)
    }

    export let name: string;
    export let alt: string;
    export let url: string;
    export let isPlain = false;
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<div class="skill-transision transition ease-in-out h-[4.5rem] w-[4.5rem] p-3 rounded-2xl bg-black bg-opacity-0 flex flex-col hover:bg-opacity-25" on:click={redirect}>
    <img class="" src={getIconFromProps()} alt={alt}/>
</div>