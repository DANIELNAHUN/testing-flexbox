<template>
<div>
    <v-row no-gutters>
        <v-card
        class="white--text px-7 py-7"
        width="250px"
        max-height="100%"
        color="#E28525">
        <v-img
        max-width="100px"
        max-height="100%"
        src="../../src/img/iconoSedan.png">
        </v-img>
        <v-card-title class="text-h5">SEDANS</v-card-title>
        <v-card-text class="caption white--text">
            Choose a sedan for its affordability and excellent fuel economy. Ideal for
            cruising int the city or on your next road trip.
        </v-card-text>
        <v-card-actions>
            <v-spacer></v-spacer>
                <v-btn rounded color="white" class="button orange--text">Learn More</v-btn>
            <v-spacer></v-spacer>
        </v-card-actions>
        </v-card>

        <v-card
        class="white--text px-7 py-7"
        width="250px"
        max-height="100%"
        color="#016972">
        <v-img
        max-width="100px"
        max-height="100%"
        src="../../src/img/iconoSuvs.png">
        </v-img>
        <v-card-title class="text-h5">SUVS</v-card-title>
        <v-card-text class="caption white--text">
            Take an SUV for its spacious interior, power, and versatility. Perfect for your
            next family vacation and off-road adventures.
        </v-card-text>
        <v-card-actions>
            <v-spacer></v-spacer>
                <v-btn rounded color="white" class="button cyan--text">Learn More</v-btn>
            <v-spacer></v-spacer>
            <v-spacer></v-spacer>
        </v-card-actions>
        </v-card>

        <v-card
        class="white--text px-7 py-7"
        width="250px"
        max-height="100%"
        color="#00403F">
        <v-img
        max-width="100px"
        max-height="100%"
        src="../../src/img/iconoLuxury.png">
        </v-img>
        <v-card-title class="text-h5">LUXURY</v-card-title>
        <v-card-text class="caption white--text">
            Cruise in the best car brands without the bloated prices. Enjoy the enhanced
            comfort of a luxury rental and arrive in style.
        </v-card-text>
        <v-card-actions>
            <v-spacer></v-spacer>
                <v-btn rounded color="white" class="button teal--text">Learn More</v-btn>
            <v-spacer></v-spacer>
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