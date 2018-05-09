<template>
    <div class="users">
        <h1>Users</h1>
        <input type="text" v-model="userId">
        <button @click="onLoadUser">Load User</button>
    </div>   
</template>


<script>
import Header from '~/components/Header.vue'
export default {
    data() {
        return {
            userId: ''
        }
    },
    methods: {
        onLoadUser() {
            this.$router.push({ name: 'users-id', params: { id: this.userId }})
        }
    },
    layout: 'users'
}
</script>