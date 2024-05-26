<script>
import RouterLink from '../components/UI/RouterLink.vue';
import Heading from '../components/UI/Heading.vue'
</script>

<template>
    <div>
        <div class="flex justify-end">
            <RouterLink :to="Inicio">
                Volver
            </RouterLink>
        </div>
       <Heading>Agregar Clientes</Heading>
    </div>
</template>


