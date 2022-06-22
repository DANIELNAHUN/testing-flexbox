<template>
    <div class="d-flex">
        <v-row justify="space-around">
            <v-card
            class="justify-md-center"
            max-width="320"
            >
            <v-img
            max-height="200"
            max-width="100%"
            src="https://images.unsplash.com/photo-1511367461989-f85a21fda167?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8NXx8cHJvZmlsZXxlbnwwfHwwfHw%3D&w=1000&q=80"
            ></v-img>
            <v-card-text class="px-8">
                <div class="text-h6 text-center font-weight-bold primary--text">Order Summary</div>
                <div class="subtitle-2 font-weight-regular text-center my-5">You can now listen to millions of song, audiobooks, and podcasts on any
                device anywhere you like!</div>
                <div class="d-flex justify-space-between">
                    <div class="d-flex align-center">
                        <v-btn
                        class="ma-2"
                        icon
                        text
                        >
                            <v-icon >mdi-music</v-icon>
                        </v-btn>
                        <div>
                            <div class="font-weight-bold">Anual Plan</div>
                            <div>$59.99/year</div>
                        </div>
                    </div>
                    <div><v-btn color="primary" text class="text-none text-decoration-underline font-weight-bold">Change</v-btn></div>
                </div>
            </v-card-text>
            <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="primary" class="text-none">Proceed to Payment</v-btn>
                <v-spacer></v-spacer>
            </v-card-actions>
            <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn color="grey" text class=" caption text-none">Cancel Order</v-btn>
                <v-spacer></v-spacer>
            </v-card-actions>

            </v-card>
        </v-row>
    </div>
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