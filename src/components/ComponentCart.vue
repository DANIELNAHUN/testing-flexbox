<template>
    <v-container>
        <v-row justify="space-around">
            <v-card
            class="justify-md-center"
            max-width="500"
            >
            <v-img
            max-height="200"
            max-width="100%"
            src="https://images.unsplash.com/photo-1511367461989-f85a21fda167?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NXx8cHJvZmlsZXxlbnwwfHwwfHw%3D&w=1000&q=80"
            ></v-img>
            <v-toolbar-title>Order Summary</v-toolbar-title>
            <h3>You can now listen to millions of song, audiobooks, and podcasts on any
                device anywhere you like!</h3>
            
            <v-btn>Proceed to Payment</v-btn>
            <v-btn>Cancel Order</v-btn>
            </v-card>
        </v-row>
    </v-container>
</template>
<script>
    export default {
        data() {
            return {}
        },
    }
</script>
<style lang="scss" scoped>
</style>