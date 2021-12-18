<template>
    <section>
        <label for="name">name:</label>
        <input type="text" name="name" v-model="userName"/>
        <label for="age">age:</label>
        <input type="text" name="age" v-model="userAge"/>
        <button @click="submitUserData">submit</button>
    </section>
</template>

<script>
export default({
    data() {
        return {
            userName: '',
            userAge: null
        }
    },
    methods: {
        submitUserData() {
            this.$emit('submit-data', this.userName, this.userAge);
        }
    }
})
</script>

<style scoped>
    section {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        height: 10em;
    }
</style>
