<script>
import Layout from "../Shared/Layout.vue";
import {Link} from "@inertiajs/vue3";

export default {
    layout: Layout,
    components: {Link},
    props: {time: Array}
}

</script>

<template>
    <h1 class="text-2xl">Users</h1>

    <div class="" style="margin-top: 1200px">
        <p>The time is {{ time }} </p>
        <Link href="/users" class="text-blue-700" preserve-scroll>refresh</Link>
    </div>
</template>

<style scoped>

</style>
