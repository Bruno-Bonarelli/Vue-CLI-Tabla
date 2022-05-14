<template>
    <div>
        <table class="table table-sm">
            <thead class="thead-light">
                <tr>
                    <th v-for="(item, i) in titulos" :key="i" scope="col">{{ item }}</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(registro, i) in registros" :key="i">
                        
                    <th v-for="(row, r) in registro" :key="r">{{row}}</th>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {
    name: 'TablaClaseCuatro',
    props: {
        titulos: {
            type: Array,
            required: true
        },
        registros: {
            type: Array,
            required: true
        },
    }
}
</script>

<style>

</style>