<template>
    <user-data @submit-data="userData"></user-data>
    <active-user 
    :user-name="userName" 
    :user-age="userAge">
    </active-user>
</template>

<script>
export default ({
    data() {
        return {
            userName: '',
            userAge: null
        }
    },
    methods: {
        userData(name, age) {
            this.userName = name;
            this.userAge = age;
        }
    }
})
</script>

<style scoped>

</style>
