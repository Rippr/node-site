<template>
    <div id="view_container">
        <section class="error first">
            <h1>404</h1>
            <h2>Page not found</h2>
            <img src="~/assets/images/icons/kabootar.png">
            <!--<p>The page you are looking for does not exist.<br>
            <a href="\">Go back</a> or contact our admin at <a href="mailto:node.dps.ggn@gmail.com">node.dps.ggn@gmail.com</a></p>-->
            <p>The Great Kabootar hath many centuries ago prophesied: <q>Thou shall never be able to conquer this link.</q></p>
            <div class="buttons">
                <nuxt-link to="/">Return to safety</nuxt-link>
                <a href="mailto:node.dps.ggn@gmail.com?subject=Need a carrier pigeon&body=Please send help.">Hire a carrier pigeon</a>
            </div>
        </section>
    </div>
</template>
<script>
export default {
    name: 'errorPage',
    props: ['error'],
    head(){
        return {
            title: 'Error!',
            meta: [{
                hid: 'Error',
                name: 'Error',
                content: 'Something went wrong.'
            }]
        }
    },
}
</script>
<style lang="sass" scoped>
@import 'assets/sass/error_page';
</style>
