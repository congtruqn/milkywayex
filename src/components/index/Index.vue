<template>
    <div>
    <div id="about">
        <div class="about_title">
            <h1 class="ps--hero__title">Get early access to the <span>ideas of tomorrow</span></h1>
            <h3 class="ps--hero__subtitle">Highly-vetted ideas and teams you can trust. Supported by industry-leading creators and funds.</h3>
            <div class="botton">
                <a class="sc_button">See upcoming sales</a>
            </div>
        </div>
        <div class="about_image">
            <img src="@/assets/images/img-2-copyright.png">
        </div>
        <div id="clear"></div>
    </div>
    <div>
        <h3 class="project_title">Upcoming Projects</h3>
        <div class="">
            <div v-for="(listproject, index) in listprojects" :key="index" class="col-lg-4 col-md-6 col-sm-6">
                <div class="project_image"><img :src="'https://admin-cloud-run-ggczm4ik6q-an.a.run.app/uploads/'+listproject.image"></div>
            </div>
        </div>
    </div>
    </div>
</template>
<script>
export default {
    data(){
        return {
            listprojects:[]
        }
    },
    methods : {
    },
    mounted () {
        this.$http.get('https://admin-cloud-run-ggczm4ik6q-an.a.run.app/getallproject',{headers: {}})
      .then(response => (this.listprojects = response.data));
    }
}
</script>
