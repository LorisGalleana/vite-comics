<script>
    export default {
        name :'AppContent',
    }
</script>

<template>
    <div class="component-container">
        <div class="container">
        --> Content go here <--
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.component-container {
    background-color: black; 
}
.container {
    @include center(horizontal);
    height: 30vh;
    color: white;
    font-weight: bold;
    font-size: 24px;
}
</style>