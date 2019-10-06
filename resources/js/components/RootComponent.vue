<template>
    <div class="container">
        {{authenticated}}
    </div>
</template>

<script>
    export default {
        props: ['authenticated'],
        mounted() {
            console.log('Component mounted.')
            console.log(this.authenticated);
        }
    }
</script>
