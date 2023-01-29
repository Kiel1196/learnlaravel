<script setup>
import {Link} from '@inertiajs/vue3'
import {ref} from 'vue'

const timer = ref( 0 )

setInterval( () => timer.value++, 1000 )

defineProps({
    message: String
})
</script>

<template>
    <Link href="/">Main Page</Link>&nbsp;
    <Link href="/hello">Show Page</Link>
    <div>Timer : {{ timer }}</div>
    <slot></slot>
</template>