<template>
    <div class="test-class">
        <h1>This is test page created by me</h1>
    </div>
</template>
  
<style lang="scss">
@use '../styles/variables.scss' as *;


@media (min-width: 1024px) {
    .test-class {
        min-height: 100vh;
        display: flex;
        align-items: center;
    }
}
</style>