<script lang="ts">
export function converteTempo(duracao: number) {

    const horas = Math.floor(duracao / 3600)
    const minutos = Math.floor((duracao % 3600) / 60)
    const segundos = duracao % 60

    const duracaoConvertida = [horas, minutos, segundos]
        .map(elemento => String(elemento).padStart(2, '0'))
        .join(":")
    return (duracaoConvertida)
}
export function converteData(data: string){
    const d = new Date(2005,4,31)
    const options={ year: 'numeric', month: 'short', day: 'numeric', };
    
    return d.toLocaleDateString('pt-BR', options).replace('de', " ")
}
</script>