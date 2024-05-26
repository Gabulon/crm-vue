<script>
import ClienteService from '../services/ClienteService';
import RouterLink from '../components/UI/RouterLink.vue';
defineProps({
        titulo: {
            type: String
        }
    })
</script>

<template>
    <div>
        <div class="flex justify-end">
            <RouterLink :to="inicio">
                Volver
            </RouterLink>
        </div>
        <Heading>{{ titulo }}</Heading>
    </div>
</template>


