<script>
import {Link} from "@inertiajs/vue3";
import NavLink from "./NavLink.vue";

export default {
    name: "Nav",
    components: {NavLink, Link}
}
</script>

<template>

    <nav class="ml-6">
        <ul class="flex list-disc space-x-4 list-inside">
            <li>
                <NavLink href="/" :active="$page.component === 'Home'">Home</NavLink>
            </li>
            <li>
                <NavLink href="/users" :active="$page.component === 'Users'">Users</NavLink>
            </li>
            <li>
                <NavLink href="/settings" :active="$page.component === 'Settings'">Settings</NavLink>
            </li>
        </ul>
    </nav>
</template>

<style scoped>

</style>
