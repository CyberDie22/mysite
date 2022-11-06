<svelte:head>
    <title>Skills</title>
</svelte:head>

<script>
    // @ts-ignore
    import Skill from '$lib/Skill.svelte'
</script>

<h1 class="text-4xl pb-2">Skills</h1>

<div class="grid grid-rows-[repeat(4,minmax(0,72px))] grid-cols-[repeat(4,minmax(0,72px))] sm:grid-rows-[repeat(2,minmax(0,72px))] sm:grid-cols-[repeat(8,minmax(0,72px))] gap-y-5 h-full w-full justify-center">
    <Skill name="kotlin" alt="Kotlin Programming Language" url="https://kotlinlang.org" />
    <Skill name="python" alt="Python Programming Language" url="https://python.org" />
    <Skill name="typescript" alt="TypeScript Programming Language" url="https://typescriptlang.org" />
    <Skill name="tailwindcss" alt="TailwindCSS" isPlain=true url="https://tailwindcss.com" />
    <Skill name="css3" alt="CSS" url="https://developer.mozilla.org/en-US/docs/Web/CSS" />
    <Skill name="java" alt="Java Programming Language" url="https://java.com" />
    <Skill name="android" alt="Android by Google" url="https://android.com" />
    <Skill name="apple" alt="Apple" url="https://apple.com" />
    <Skill name="cplusplus" alt="C++ Programming Languge" url="https://en.wikipedia.org/wiki/C%2B%2B" />
    <Skill name="docker" alt="Docker" url="https://docker.com" />
    <Skill name="jetbrains" alt="JetBrains" url="https://www.jetbrains.com" />
    <Skill name="linux" alt="Linux" url="https://kernel.org" />
    <Skill name="rust" alt="Rust" isPlain=true url="https://rust-lang.org" />
    <Skill name="svelte" alt="Svelte" url="https://svelte.dev" />
</div>