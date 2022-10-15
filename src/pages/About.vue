<template>
    <div>
        <Navbar />

        <section class="about">

            <h1 class="heading"> about <span>series</span> </h1>

            <div class="row">

                <div class="info-container">

                    <h1>info</h1>

                    <div class="box-container">

                        <div class="box">
                            <h3> <span>Genre : </span> {{Genre}} </h3>
                            <h3> <span>Based on : </span> {{Based}} </h3>
                            <h3> <span>Written by : </span> {{Written}} </h3>
                            <h3> <span>Directed by : </span> {{Directed}} </h3>
                        </div>

                    </div>

                </div>

                <div class="count-container">

                    <div class="box" v-for="e in Release" :key="e.Original">
                        <h3>{{e.Original}}</h3>
                        <p>{{e.ex}}</p>
                    </div>
                </div>

            </div>

        </section>

    </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import axios from 'axios'

export default {
    components: { Navbar },
    data() {
        return {
            Genre: 'Coming-of-age,Romantic comedyTeen,drama',
            Based: 'Heartstopper',
            Written: 'Alice Oseman',
            Directed: 'Euros Lyn',

            study: [],

            Release: [{
                Original: 'Original network',
                ex: 'Netflix'
            }, {
                Original: 'Picture format',
                ex: '4K UHDTV'
            }, {
                Original: 'Audio format',
                ex: 'Surround'
            }, {
                Original: 'Original release',
                ex: '22 April 2022'
            }]

        }
    }

}
</script>

<style>


</style>