<script>
import { FormKit} from '@formkit/vue'
import RouterLink from '../components/UI/RouterLink.vue';
import Heading from '../components/UI/Heading.vue';
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

        <div class="mx-auto mt-10 bg-white shadow">
            <div class="mx-auto md:w-2/3 py-20 px-6">
                <FormKit type="form">
                    <FormKit
                    type="text"
                    label="Nombre"
                    placeholder="Nombre de Cliente"
                    validation="required"
                    :validation-messages="{required:'El nombre del Cliente es Obligatorio'}"
                 />
                    <FormKit
                    type="text"
                    label="Apellido"
                    placeholder="Apellido de Cliente"
                    validation="required"
                    :validation-messages="{required:'El apellido del Cliente es Obligatorio'}"
                 />
                    <FormKit
                    type="email"
                    label="Email"
                    placeholder="Email de Cliente"
                    validation="required|email"
                    :validation-messages="{required:'El email del Cliente es Obligatorio', email:'Coloca un email valido'}"
                 />
                    <FormKit
                    type="text"
                    label="Telefono"
                    placeholder="Telefono: XXX-XXX-XXXX"
                    validation="*matches:/^[0-9]{3}-[0-9]{3}-[0-9]{4}$/"
                    :validation-messages="{matches:'El formato no es valido'}"
                 />
                 </FormKit>
            </div>
        </div>
    </div>
</template>

<style>
.formkit-wrapper{
    max-width: 100%;
}

</style>


