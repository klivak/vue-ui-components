<template>
    <section class="section section-gallery">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <h3> {{ title }} </h3>
                </div>
                <div class="col-md-12">
                    {{ description }}
                </div>
            </div>
            <div class="row">
                <div class="gallery-images">

                    <div v-for="image in images"
                         :key="image.id"
                         class="image-item"
                    >

                        <div class="image-content"
                             :style="{ backgroundImage: 'url(' + image.thumbnail + ')' } "
                        >

                        </div>

                    </div>

                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        props: {
            title: {
                type: String,
                default: 'Gallery'
            },
            description: {
                type: String
            },
            images: {
                type: Array
            }
        },
        data() {
            return {}
        }
    }
</script>

<style scoped>

</style>