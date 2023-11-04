<template>
    <div>
        <Navbar />
        <section class="home">
            <div class="image">
                <img src="images/profile.png" alt="">
            </div>

            <div class="content">
                <h3>hi, i am {{ name }}</h3>
                <span>{{motto}}</span>
                <p>{{content}}</p>
                <a href="about.html" class="btn"> about me <i class="fas fa-user"></i> </a>
            </div>
        </section>
    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components : { Navbar },
    data() { 
        return { 
            name: 'Sita Gantanaprasert',
            motto: 'Sleep is my habit.',
            content: 'I study on Multimedia Engineering at Bangkok University.Now I 18 year old.'
        } 
    }
}
</script>

<style>

</style>