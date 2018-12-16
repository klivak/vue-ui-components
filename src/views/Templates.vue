<template>
    <div class="page page-templates">
        <h1>This is an templates page</h1>

        <banner :bg-image="bannerImage"
                :title="bannerTitle"
                :description="bannerDescription"
        ></banner>

    </div>
</template>

<script>

    import data from '../data'
    // const data = require('../data.json');

    import banner from '@/components/sections/Banner'

    export default {
        data() {
            return {
                data,
                bannerImage: data.banner.image,
                bannerTitle: data.banner.title,
                bannerDescription: data.banner.description,
            }
        },
        mounted() {
            console.log(this.bannerImage);
        },
        components: {
            banner
        }
    }
</script>