<template>
    <section class="section section-modal">

        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <button class="btn btn-open"
                            @click="openModal()"
                    >
                        {{ btnText }}
                    </button>
                </div>
            </div>
        </div>

        <!-- modal container -->

        <div class="modal-overlay"
             ref="modal"
        >
            <div class="modal-content">
                <div class="modal-header">
                    <h3>title</h3>
                    <button class="btn-close" @click="closeModal()">X</button>
                </div>
                <div class="modal-body">
                    it is modal content
                </div>
            </div>


        </div>

    </section>
</template>

<script>
    export default {
        props: {
            btnText: {
                type: String,
                default: 'Open'
            }
        },
        data() {
            return {}
        },
        methods: {
            openModal() {
                this.$refs.modal.classList.add("active");
            },
            closeModal() {
                this.$refs.modal.classList.remove("active");
            }
        }
    }
</script>

<style scoped>

</style>