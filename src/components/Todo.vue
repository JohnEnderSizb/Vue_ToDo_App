<template>
    <div>
        <div v-for="todo in todos" :key="todo.id">
            <h3>{{ todo.title }}</h3>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Todo",
        props: ["todos"]
    }
</script>

<style scoped>

</style>
