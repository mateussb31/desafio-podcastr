

<template>
    <div>
        <table>
            <colgroup>
                <col span="1" style="width: 40%;">
                <col span="1" style="width: 20%;">
                <col span="1" style="width: 20%;">
                <col span="1" style="width: 20%;">
            </colgroup>
            <caption> Todos os epsodios</caption>
            <thead>
                <tr>
                    <th>PODCAST</th>
                    <th>INTEGRANTES</th>
                    <th>DATA</th>
                    <th>DURAÇÃO</th>
                    <th></th>
                </tr>
            </thead>
            <tbody v-for="ep, index in listaEpsodios.slice(2)" :key="ep.id">
                <tr v-if="index < 5">
                    <p>
                        <img :src="ep.thumbnail" />
                    <p style="float: left;margin: 22px 0px; text-overflow: ellipsis;overflow: hidden;max-width: 80%;">
                        {{ ep.title }}</p>
                    </p>
                    <td> {{ ep.members }}</td>
                    <td> {{ converteData(ep.published_at.split(" ")[0]) }}</td>
                    <td> {{converteTempo(ep.file.duration)}}</td>
                    <td><button></button></td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script lang="ts">
import { converteTempo,converteData } from "@/utils/conversor.vue";
import epsodes from "../assets/epsodes.json"

export default {
    data() {
        return {
            listaEpsodios: epsodes
        }
    },
    methods: {
        converteTempo,
        converteData,
    }
}
</script>


<style scoped>
caption {
    font-size: 20px;
    line-height: 20px;
    text-align: left;
    margin-bottom: 32px;
}

table {
    width: 100%;
    text-align: left;
    vertical-align: center;
    border-collapse: collapse;
}

div {
    margin: 32px 64px 9px;
}

thead {
    color: #AFB2B1;
    border-bottom: 1px solid #E6E8EB;
}

tr {
    border-bottom: 1px solid #E6E8EB;
    vertical-align: center;
}

img {
    float: left;
    width: 40px;
    height: 40px;
    border-radius: 8px;
    margin: 12px 16px 12px 0px;
}
</style>