<template>
    <div>
        <Navbar />
        <section class="home">
            <div class="image">
                <img src="images/profile.png" alt="">
            </div>
            <div class="content">
                <h3>{{name}}</h3>
                <span>{{motto}}</span>
                <p>{{content}}</p>
                <router-link to="/about" class="btn"> about series <i class="fas fa-user"></i> </router-link>
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
            name: 'Heartstopper',
            motto: 'Boy meets Boy, Boys become friends, Boys fall in love',
            content: 'Teens Charlie and Nick discover their unlikely friendship might be something more as they navigate school and young love in this coming-of-age series.'
        }
     }
}
</script>

<style>

</style>