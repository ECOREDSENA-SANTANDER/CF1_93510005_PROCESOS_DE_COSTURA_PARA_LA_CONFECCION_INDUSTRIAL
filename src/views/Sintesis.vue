<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p Se exponen los conocimientos esenciales para comprender los procesos de confección industrial desde una perspectiva técnica y operativa; su desarrollo permite reconocer la relación existente entre las características de las prendas, los materiales utilizados, la maquinaria requerida, la documentación técnica y las condiciones de seguridad y salud en el trabajo. Estos conocimientos constituyen la base para ejecutar procesos de confección con criterios de calidad, eficiencia y prevención de riesgos en el entorno productivo.

    .row.justify-content-center
      .col-lg-10.mb-5.bgs.p-4.brad
        figure
          img(src="@/assets/curso/sintesis.svg", alt="La síntesis organiza los contenidos del componente en cuatro ejes temáticos: las tipologías de prendas de vestir, que incluyen sus componentes, gamas de mercado y textiles; la maquinaria de confección industrial, orientada al manejo, aplicaciones, insumos y mantenimiento preventivo; las fichas técnicas, abordadas desde su definición, tipos y aplicación; y la seguridad y salud en el puesto de trabajo, enfocada en la ergonomía y el procedimiento para el reporte de incidentes. Estos temas se articulan para favorecer la comprensión integral de los procesos propios de la confección industrial. ")
      .col-auto
        a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/bullets/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
