<template>
    <div>
        <Navbar />
        <section class="projects">
            <h1 class="heading"> <span>my</span> projects </h1>
            <h3>{{ project_name }}</h3>
            <p>{{ project_detail }}</p>
            <div class="box-container">
                <iframe width="720" height="405" src="https://www.youtube.com/embed/603Hc7ycIS0"
                    title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; 
            gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </section>
    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components: { Navbar },
    data(){
        return{
            project_name: 'Untouchable_Door',
            project_detail: 'ออกแบบประตูที่ไร้การสัมผัสเพื่อป้องกันการติดต่อของเชื้อโควิท19',
        }
    }
}
</script>

<style>

</style>