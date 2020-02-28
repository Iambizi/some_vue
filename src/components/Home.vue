<template>
    <div>
        <Hero />
        <Skills />
        <Projects />
    </div>
</template>

<script>
import Hero from './components/Home';
import Skills from './components/Skills';
import Projects from './components/Projects';
    export default {
        components: {
            Hero,
            Skills,
            Projects
        },
    }
</script>

<style lang="scss" scoped>

</style>