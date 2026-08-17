<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5.mb-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 4
      h1 Seguridad y salud en el puesto de trabajo

    .row.justify-content-center.mb-5.bg02.g-0(data-aos="zoom-in-left")
      .col-lg-4.p-0
        img.w-100.h-100.d-block.object-fit-cover.d-none.d-lg-block(src='@/assets/curso/temas/t4/img01.png', alt='')
      .col-lg-8
        .row.mb-0.p-5
          .col-lg-2.mb-3.col-4.col-md-3
            img.wid15(src='@/assets/curso/temas/t4/img02.png', alt='')
          .col-lg-12
            p.mb-0 La seguridad y salud en el trabajo constituye un eje transversal de la actividad productiva en el sector de la confección. Su incorporación en los procesos no responde únicamente a obligaciones normativas, sino a la necesidad de garantizar condiciones laborales que protejan la integridad física y mental de quienes participan en la cadena de producción. El conocimiento de los factores de riesgo presentes en el entorno de confección, así como la aplicación de medidas preventivas y protocolos de actuación ante eventos adversos, forma parte de las competencias esenciales del técnico en este campo.

    .row.justify-content-start.mb-4(data-aos="zoom-in-left")
      .col-sm-12.col-lg-7
        .d-flex.align-items-center
          img.w-card-icon(src="@/assets/curso/temas/t3/ico.svg")
          h3.bg03.py-2.w-card-text Tipos de riesgos laborales, de postura y de movimientos 

    p Los riesgos laborales en el entorno de confección se clasifican según su naturaleza y el mecanismo a través del cual afectan la salud. Su identificación sistemática es el punto de partida de cualquier estrategia de prevención eficaz dentro del Sistema de Gestión de Seguridad y Salud en el Trabajo (SG-SST).

    .row.justify-content-start.mb-4(data-aos="zoom-in-left")
      .col-sm-12.col-lg-7
        .d-flex.align-items-center
          img.w-card-icon(src="@/assets/curso/temas/t3/ico.svg")
          h3.bg03.py-2.w-card-text Riesgos físicos

    p Los riesgos físicos se originan en las condiciones ambientales del lugar de trabajo y actúan sobre el organismo sin necesidad de contacto directo con la fuente. En los puestos de confección, los de mayor prevalencia son los siguientes:

    .row.justify-content-center.cursor-pointer.mb-5(data-aos="zoom-in-left")
        .col-xl-4.col-md-7.col-11.mb-4.mb-xl-0
          .crd_hover_txt(@mouseover="mostrarIndicador = false")
            .indicador--hover(v-if="mostrarIndicador")
            .crd_hover_txt--img
              figure
                img(src="@/assets/curso/temas/t4/1.png", alt="")
            .crd_hover_txt--body
              h4.mb-4.d-flex.align-items-center
                span.icono-circulo.me-3
                  span.flecha
                | Ruido
              p.mb-0 Las máquinas de coser industriales generan niveles sonoros que, ante exposición prolongada sin protección auditiva adecuada, producen deterioro auditivo de carácter progresivo e irreversible. La normativa colombiana establece un límite de 85 decibeles para exposición continua durante una jornada de ocho horas, tal como lo dispone la Resolución 8321 de 1983 del Ministerio de Salud.
        
        .col-xl-4.col-md-6.col-11.mb-4.mb-xl-0
          .crd_hover_txt(@mouseover="mostrarIndicador = false")
            .indicador--hover(v-if="mostrarIndicador")
            .crd_hover_txt--img
              figure
                img(src="@/assets/curso/temas/t4/2.png", alt="")
            .crd_hover_txt--body
              h4.mb-4.d-flex.align-items-center
                span.icono-circulo.me-3
                  span.flecha
                | Iluminación deficiente
              p.mb-0 La insuficiencia lumínica en el puesto de trabajo incrementa la probabilidad de errores en la costura, genera fatiga visual acumulada y aumenta el riesgo de accidentes. Cada puesto debe contar con iluminación localizada sobre el área de costura, complementaria a la iluminación general del espacio.
        
        .col-xl-4.col-md-6.col-11.mb-4.mb-xl-0
          .crd_hover_txt(@mouseover="mostrarIndicador = false")
            .indicador--hover(v-if="mostrarIndicador")
            .crd_hover_txt--img
              figure
                img(src="@/assets/curso/temas/t4/3.png", alt="")
            .crd_hover_txt--body
              h4.mb-4.d-flex.align-items-center
                span.icono-circulo.me-3
                  span.flecha
                | Temperatura
              p.mb-0 Las condiciones térmicas inadecuadas (tanto la exposición a calor excesivo como a corrientes de aire frío) afectan la capacidad de concentración y pueden desencadenar afecciones musculoesqueléticas en trabajadores expuestos de forma continua.
    .row.justify-content-start.mb-4(data-aos="zoom-in-left")
      .col-sm-12.col-lg-7
        .d-flex.align-items-center
          img.w-card-icon(src="@/assets/curso/temas/t3/ico.svg")
          h3.bg03.py-2.w-card-text Riesgos mecánicos

    p Los riesgos mecánicos se derivan del contacto directo o indirecto con la maquinaria, las herramientas de corte y los materiales del proceso productivo. Los eventos de mayor frecuencia en el sector son:























</template>

<script>
export default {
  name: 'Tema4',
  data: () => ({
    // variables de vue
  }),
}
</script>

<style lang="sass"></style>
