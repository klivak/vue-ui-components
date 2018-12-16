<template>
    <div class="page page-templates">
        <h1>This is an templates page</h1>

        <banner :bg-image="bannerImage"
                :title="bannerTitle"
                :description="bannerDescription"
                class="d-none"
        ></banner>

        <hr>

        <modal :btn-text="modal.buttonText"
        ></modal>

        <hr>

        <gallery
                :title="gallery.title"
                :description="gallery.description"
                :images="gallery.images"

        >
        </gallery>

    </div>
</template>

<script>

    import data from '../data'
    // const data = require('../data.json');

    import banner from '@/components/sections/Banner';
    import modal from '@/components/sections/Modal';
    import gallery from '@/components/sections/Gallery';

    export default {
        data() {
            return {
                data,
                bannerImage: data.banner.image,
                bannerTitle: data.banner.title,
                bannerDescription: data.banner.description,
                modal: {
                    buttonText: data.modal.btnText
                },
                gallery: {
                    title: data.gallery.title,
                    description: data.gallery.description,
                    images: data.gallery.images
                }
            }
        },
        mounted() {
            console.log('data', data);
        },
        components: {
            banner,
            modal,
            gallery
        }
    }
</script>