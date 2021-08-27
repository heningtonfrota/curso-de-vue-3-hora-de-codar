<template>
    <PrimeiroCompomente />
    <LifeCycle />
</template>

<script>
    import PrimeiroCompomente from './components/PrimeiroComponente.vue'
    import LifeCycle from './components/LifeCycle.vue'
    export default {
        name: 'App',
        components: {
            PrimeiroCompomente,
            LifeCycle
        }
    }
</script>

<style>

</style>