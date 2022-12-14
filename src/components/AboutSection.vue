<script setup>
</script>

<template>
    <section class="about">
        <div class="container">
            <div class="about-inner">
                About section
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/variables.scss' as *;


@media (min-width: 1024px) {
    .about {
        min-height: 100vh;
        display: flex;
        align-items: center;
    }
}
</style>