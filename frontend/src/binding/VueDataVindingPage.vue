<template>
<div>
    <p>Hello {{ message }}</p>
    <p>길이: {{ message.length }}</p>
    <p>list[2]: {{list[2]}}</p>
    <p>num1: {{number}}</p>

    <input type="text" v-model="num1">{{num1}}

</div>
</template>

<script>
export default {
    name: "VueDataVindingPage",
    data () {
        return {
            message: 'Vue programming',
            list: ['apple', 'grape', 'watermelon'],
            show: true,
            number: 1
        }
    }
}
</script>

<style scoped>

</style>