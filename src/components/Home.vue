<template>
    <div>
        <Nav />
        <Hero />
        <Skills />
        <Projects />
        <Footer />
    </div>
</template>

<script>
    import Nav from './Nav';
    import Hero from './Hero';
    import Skills from './Skills';
    import Projects from './Projects';
    import Footer from './Footer';
        export default {
            components: {
                Nav,
                Hero,
                Skills,
                Projects,
                Footer
            },
        }
</script>

<style lang="scss" scoped>
        body{
        opacity: 1;
        transition: 2s opacity;
        .fade-out {
            opacity: 0;
            transition: none;
        }
    }
</style>