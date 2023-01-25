<script setup>
import {Link} from '@inertiajs/vue3'

defineProps({
    message: String
})
</script>

<template>
    <Link href="/">Main Page</Link>&nbsp;
    <Link href="/hello">Show Page</Link>
    <slot></slot>
</template>