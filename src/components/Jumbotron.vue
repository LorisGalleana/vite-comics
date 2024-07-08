<script>
    export default {
        name :'Jumbotron',
        
    }
</script>




<template>
    <div class="jumbotron"></div>
</template>





<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.jumbotron {
    height: 300px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}


</style>