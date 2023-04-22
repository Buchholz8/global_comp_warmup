<template>
    <div>
        <button @click="post"></button>
    </div>
</template>

<script>
    export default {
        methods : {
            post: function ( ) {
                this.$root.$emit(`post` , `congrates you have posted`)
            }
        }
        
    }
</script>

<style scoped>

</style>