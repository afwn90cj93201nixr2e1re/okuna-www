<template>
    <section class="hero is-white">
        <div class="hero-body has-text-centered">
            <div class="container">
                <div class="columns is-centered is-vcentered">
                    <div class="column">
                        <router-link to="about-us" class="button is-rainbow is-rounded is-medium">
                            {{ $t('meet_the_team.title') }}
                        </router-link>
                    </div>
                    <div class="column">
                        <div class="columns is-centered is-mobile">
                            <div class="column is-narrow" style="margin-left: -10px;">
                                <div class="home-team">
                                    <figure class="image is-64x64 home-team-figure" v-for="teamImage in teamImages">
                                        <img class="is-rounded" :src="teamImage" alt="Image">
                                    </figure>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import teamImage1 from './assets/joel-min.jpg';
    import teamImage2 from './assets/jaya-min.png';
    import teamImage3 from './assets/phil-min.jpg';
    import teamImage4 from './assets/vincent-min.jpeg';
    import teamImage5 from './assets/robin-min.png';
    import teamImage6 from './assets/nathalie-min.png';
    import teamImage7 from './assets/shantanu-min.jpg';

    export default{
        name: 'ob-meet-the-team',
        data(){
            return {
                teamImages:[
                    teamImage5,
                    teamImage4,
                    teamImage2,
                    teamImage3,
                    teamImage1,
                    teamImage6,
                    teamImage7
                ]
            }
        }
    }
</script>
