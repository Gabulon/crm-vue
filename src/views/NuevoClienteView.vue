<script>
    import {RouterLink} from 'vue-router'
</script>

<template>
    <div>
        <div>
            <RouterLink :to="{name:'home'}">
                Volver
            </RouterLink>
        </div>
        <h1 class="text-4xl font-extrabold text-slate-500">Agregar Clientes</h1>
    </div>
</template>


