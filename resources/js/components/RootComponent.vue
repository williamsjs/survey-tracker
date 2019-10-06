<template>
    <div class="container">
        <template v-if="authenticated">
            authenticated
        </template>
        <template v-else>
            not Authenticated
        </template>
    </div>
</template>

<script>
    export default {
        props: ['authenticated'],
        mounted() {
            this.authenticated = JSON.parse(this.authenticated);
        }
    }
</script>
