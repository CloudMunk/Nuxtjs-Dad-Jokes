<template>
    <div>
        <form @submit.prevent="onSubmit">
            <input type="text" v-model="text" placeholder="Search jokes">
            <input type="submit" value="Seacr Jokes">
        </form>
    </div>
</template>

<script>
export default {
    name: 'Search Jokes',
    data() {
        return {
            text: ''
        }
    },
    methods: {
        onSubmit() {
            this.$emit('search/text', this.text)
            this.text = ''
        }
    }
}
</script>

<style scoped>

</style>