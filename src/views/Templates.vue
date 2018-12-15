<template>
    <div class="page page-templates">
        <h1>This is an templates page</h1>

        <banner bg-image="'/static/images/bg-image-min.jpg'"
                title="Banner"
                description="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi quam tellus, lacinia vel
                neque a, viverra rutrum sem. Nulla gravida."
        ></banner>

    </div>
</template>

<script>

    import banner from '@/components/sections/Banner'

    export default {
        data() {
            return {}
        },
        components: {
            banner
        }
    }
</script>