<template>
    <Page actionBarHidden="true">
        

       
    </Page>
</template>

<script>
    import Login from "./Login";

    export default {
        data() {
            return {
                
            };
        },
        methods: {
            logout() {
                this.$backendService.logout();
                this.$navigateTo(Login, {
                    clearHistory: true
                });
            }
        }
    };
</script>

<style>
</style>
