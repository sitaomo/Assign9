<template>
    <div>
        <Navbar />

        <section class="about">

            <h1 class="heading"> about <span>me</span> </h1>

            <div class="row">

                <div class="info-container">

                    <h1>personal info</h1>

                    <div class="box-container">

                        <div class="box">
                            <h3> <span>name : </span> {{name}} </h3>
                            <h3> <span>age : </span> {{age}} </h3>
                            <h3> <span>email : </span> {{email}} </h3>
                            <h3> <span>address : </span> {{address}} </h3>
                        </div>

                        <div class="box">
                            <h3> <span>Student : </span> available </h3>
                            <h3> <span>skill : </span> Sleep </h3>
                            <h3> <span>experience : </span> 0 years </h3>
                            <h3> <span>language : </span> thai </h3>
                        </div>

                    </div>

                    <a href="/profilewithcss/files/resume.pdf" class="btn"> download CV <i class="fas fa-download"></i>
                    </a>

                </div>

                <div class="count-container">

                    <div class="box">
                        <h3>5+</h3>
                        <p>years of experience</p>
                    </div>

                    <div class="box">
                        <h3>10+</h3>
                        <p>happy clients</p>
                    </div>

                    <div class="box">
                        <h3>20+</h3>
                        <p>project completed</p>
                    </div>

                    <div class="box">
                        <h3>5+</h3>
                        <p>Certificates</p>
                    </div>

                </div>

            </div>

        </section>

        <!-- about section ends -->

        <!-- skills section starts  -->

        <section class="skills">

            <h1 class="heading"> <span>my</span> skills </h1>

            <div class="box-container">
                <div class="box">
                    <img src="images/icon-1.png">
                    <h3>html</h3>
                </div>
                <div class="box">
                    <img src="images/icon-2.png">
                    <h3>css</h3>
                </div>
                <div class="box">
                    <img src="images/icon-3.png">
                    <h3>javascript</h3>
                </div>
                <div class="box">
                    <img src="images/icon-4.png">
                    <h3>sass</h3>
                </div>
                <div class="box">
                    <img src="images/icon-5.png">
                    <h3>angular</h3>
                </div>
                <div class="box">
                    <img src="images/icon-6.png">
                    <h3>react.js</h3>
                </div>
            </div>

        </section>

        <!-- skills section ends -->

        <!-- education section starts  -->

        <section class="education">

            <h1 class="heading"> <span>my</span> experience </h1>

            <div class="box-container">

                <div class="box" v-for="e in experiences" :key="e.years">
                    <i class="fas fa-briefcase"></i>
                    <span>{{e.years}}</span>
                    <h3>{{e.company}}</h3>
                    <p>{{e.jobs}}.</p>
                </div>
            </div>

        </section>
    </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
export default {
    components: { Navbar },
    data(){
        return{
            experiences:[{
                years: '2016 - 2017',
                company: 'INTER EXPRESS LOGISTICS PRIVATE LIMITED',
                jobs: 'Assist the system analyst in conduct analysis, architecture, design database model for the new application.',
            },{
                years: '2017 - 2018',
                company: 'PTT Digital Solutions Company Limited',
                jobs: 'Front-end coding to develop web applications follows by mock-up screen design. And back-end coding and test to configuration workflows and business processes.',
            },{
                years: '2018 - 2018',
                company: 'Thai Beverage PLC',
                jobs: 'Develop new features to facilitate related procedures and tools if necessary, Troubleshoot, test, and maintain the core product software and databases to ensure strong optimization and functionality.',
            },{
                years: '2019 - 2020',
                company: 'Cigna',
                jobs: 'Assist the system analyst in conduct analysis, architecture, design database model for the new application.',
            },{
                years: '2019 - 2020',
                company: 'EMETWORKS',
                jobs: 'Develop new features to facilitate related procedures and tools if necessary.',
            },{
                years: '2020 - 2021',
                company: 'uTech Solutions',
                jobs: 'Assist the system analyst in conduct analysis, architecture, design database model for the new application.',
            }],
            name: 'Sita Gantanaprasert',
            age: '19',
            email: 'sita.gant@gmail.com',
            address: 'Nontaburi, Thailand 11110'
        }
    }
}
</script>

<style>

</style>