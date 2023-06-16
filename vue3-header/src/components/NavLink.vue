<template>
    <div>
        <a :href="link">{{ name }}</a>
    </div>
</template>

<script>
export default {
    name: 'NavLink',
    props: {
        name: {
            type: String,
        },
        link: {
            type: String,
        },
    },
}
</script>

<style scoped>
</style>