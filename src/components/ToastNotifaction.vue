<template>
    <div>
        <h2> {{toast}} </h2>
        <button @click="clear" v-if="toast != undefined"> Clear Notifactions </button>
    </div>
</template>

<script>
    export default {
        data( ) {
            return{
                toast: undefined
            }
        },
        methods: {
            handler: function(details) {
                this.toast = details
            },
            clear: function() {
                this.toast = undefined
            }
        },
        mounted() {
            this.$root.$on(`toast_notify` , this.handler);
        }
    }
</script>

<style scoped>

</style>