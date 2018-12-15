<template>
    <section class="section section-banner"
             :style="{ backgroundImage: 'url(' + bgImage + ')' }"
    >
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <h3 class="title" v-if="title !== 0">
                        {{ title }}
                    </h3>
                    <div class="description" v-if="description !== 0">
                        {{ description }}
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        props: {
            bgImage: {
                type: String
            },
            title: {
                type: String,
                default: ''
            },
            description: {
                type: String,
                default: ''
            }
        },
        data() {
            return {}
        }
    }
</script>

<style scoped>

</style>