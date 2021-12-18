<template>
    <section>
        <h2> {{ userName }} </h2>
        <h3> {{ userAge }} </h3>
    </section>
</template>

<script>
export default ({
    props: ['userName', 'userAge']
})
</script>

<style scoped>
    section {
        text-align: center;
        margin-top: 5em;
    }
</style>
