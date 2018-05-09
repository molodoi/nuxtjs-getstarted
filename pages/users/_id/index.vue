<template>
    <div class="user">
        <h1>Single user {{ $route.params.id }}</h1>
    </div>  
</template>

<script>
import Header from '~/components/Header.vue'
export default {
    // Executer avant le rendu : Valide les données de l'url, comme des requirements.
    validate(data) {
        return /^\d+$/.test(data.params.id)
    },
    layout: 'users'
}
</script>