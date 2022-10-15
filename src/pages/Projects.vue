<template>
    <div>
        <Navbar />
        <section class="projects">
            <h1 class="heading"> <span>Heartstopper</span> Netflix </h1>
            <h3>{{project_name}}</h3>
            <p>{{project_detail}}</p>
            <div class="box-container">
                <iframe width="760" height="515" src="https://www.youtube.com/embed/FrK4xPy4ahg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </section>
    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components: { Navbar },
    data() { 
        return { 
            project_name: 'Heartstopper | Official Trailer | Netflix',
            project_detail: 'Love meets doubt. Fear meets joy. Boy meets boy. HEARTSTOPPER, an eight chapter story about life, love and everything in between. Based on the bestselling graphic novels from Alice Oseman.'
        }
     }
}
</script>

<style>

</style>