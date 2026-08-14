<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      // Para cuestionario usar: <ActividadController :cuestionario="cuestionario"/>
      // Para parrafo usar: <ActividadController :parrafo="parrafo"/>
      #Actividad                
      <ActividadController :cuestionario="cuestionario"/>
  
  </template>

<script>
import ActividadController from '@ecored-sena/boulder-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Maquinaria y tipología de prendas',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> verificar la apropiación conceptual y técnica de los contenidos relacionados con maquinaria en la confección, tipología de prendas y seguridad y salud en el puesto de trabajo.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto:
            '¿Cuál es el propósito principal de los procesos de costura industrial?',
          imagen: '@/assets/actividad/imagen1.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Decorar prendas mediante técnicas manuales sin maquinaria.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Unir, reforzar, terminar y complementar piezas de una prenda.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Diseñar figurines para definir colecciones de temporada.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Clasificar colores según tendencias del sistema de la moda.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 2,
          texto:
            'En confección industrial, ¿por qué es importante alistar la maquinaria antes de iniciar una operación?',
          imagen: '@/assets/actividad/imagen2.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Porque permite reemplazar la ficha técnica por instrucciones verbales.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Porque evita el uso de agujas, hilos y accesorios especializados.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Porque ayuda a preparar condiciones técnicas, insumos y parámetros de operación.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Porque elimina la necesidad de revisar la calidad del producto terminado.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 3,
          texto:
            '¿Cuál de las siguientes operaciones corresponde a un proceso de costura industrial?',
          imagen: '@/assets/actividad/imagen3.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Costura recta, fileteado, recubrimiento y presillado.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Ilustración, bocetación, diagramación y rotulación.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Teñido, estampado, sublimación y fotografía.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Empaque, transporte, venta y exhibición comercial.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 4,
          texto:
            '¿Qué aspecto técnico de una prenda determina el tipo de aguja, hilo, puntada y maquinaria que debe emplearse?',
          imagen: '@/assets/actividad/imagen4.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'El nombre comercial de la empresa fabricante.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'El color principal de la colección.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'El estilo publicitario de la marca.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'El material utilizado en la confección.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 5,
          texto:
            '¿Cuál de las siguientes opciones corresponde a prendas superiores?',
          imagen: '@/assets/actividad/imagen05.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Pantalones, faldas, <i>shorts</i> y bermudas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Overoles, vestidos enterizos y batas largas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Camisas, blusas, camisetas y chaquetas.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Cinturones, gorras, bufandas y bolsos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 6,
          texto:
            '¿Qué componentes se encuentran con mayor frecuencia en una camisa?',
          imagen: '@/assets/actividad/imagen6.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Delanteros, espalda, mangas, cuello, puños y tapeta.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Pretina, pasadores, tiro, entrepierna y bota.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Forro interno, hombreras, entretela pesada y solapa.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Capucha, cordón, broche, resorte y cargaderas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 7,
          texto:
            '¿Qué función cumplen los componentes de entretela en una prenda?',
          imagen: '@/assets/actividad/imagen7.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Sustituir el textil principal durante el proceso de corte.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Aportar firmeza, cuerpo o estabilidad a partes específicas.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Eliminar la necesidad de utilizar costuras de refuerzo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Cambiar la talla final después del proceso de ensamble.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 8,
          texto: '¿Cuál es la función técnica de un bolsillo en una prenda?',
          imagen: '@/assets/actividad/imagen8.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Servir como pieza de almacenamiento o detalle funcional.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Reemplazar la unión principal entre delantero y espalda.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Sustituir el uso de botones, ojales y cierres.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Determinar exclusivamente la talla comercial de la prenda.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 9,
          texto:
            '¿Qué pieza se utiliza para rematar aberturas, reforzar bordes o ubicar botones y ojales?',
          imagen: '@/assets/actividad/imagen9.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Canesú.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Pretina.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Manga.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Tapeta.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 10,
          texto:
            '¿Cuál sistema de cierre está compuesto por dos cintas compatibles que se adhieren entre sí por contacto?',
          imagen: '@/assets/actividad/imagen10.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Cremallera.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Alamar.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Velcro.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Cordón.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },
        {
          id: 11,
          texto: '¿Qué son las gamas de mercado en el sistema de la moda?',
          imagen: '@/assets/actividad/imagen1.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Listados de maquinaria organizados por velocidad y consumo eléctrico.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Métodos de puntada definidos por tipo de aguja industrial.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Clasificaciones de prendas según exclusividad, producción, precio y público objetivo.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Formatos de control usados únicamente en mantenimiento preventivo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 12,
          texto: '¿Qué se entiende por fibras textiles?',
          imagen: '@/assets/actividad/imagen2.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Piezas metálicas que permiten regular la tensión del hilo.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Elementos básicos que conforman hilos, tejidos y telas.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Accesorios utilizados para ajustar máquinas de ciclo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Documentos técnicos empleados en control de calidad.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 13,
          texto:
            '¿Cuál de las siguientes opciones corresponde a una fibra natural de origen vegetal?',
          imagen: '@/assets/actividad/imagen3.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Poliéster.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Nailon.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Algodón.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Acrílico.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 14,
          texto:
            '¿Qué tipo de tejido se recomienda con frecuencia para prendas que requieren elasticidad y recuperación?',
          imagen: '@/assets/actividad/imagen4.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Tejido de punto.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Tejido de raso.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Tejido de tafetán.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Tejido de sarga.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 15,
          texto: '¿Para qué sirve calcular el aprovechamiento textil?',
          imagen: '@/assets/actividad/imagen05.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Para definir la gama comercial de una prenda.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Para optimizar el uso del material y reducir desperdicios.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Para reemplazar la selección de maquinaria industrial.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Para eliminar los márgenes de costura del patrón.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 16,
          texto:
            '¿Cuál de las siguientes acciones corresponde a una práctica segura en el puesto de costura?',
          imagen: '@/assets/actividad/imagen6.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Manipular la aguja con la máquina encendida.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Mantener orden, postura adecuada y elementos de protección.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Trabajar sin reportar ruidos o fallas de la máquina.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Ubicar materiales pesados sin control en zonas de paso.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 17,
          texto:
            '¿Cuál máquina se recomienda para realizar costuras de ensamble en tejido plano?',
          imagen: '@/assets/actividad/imagen7.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Máquina plana de una aguja.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Máquina fileteadora industrial.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Máquina botonadora de ciclo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Máquina ojaladora automática.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 18,
          texto:
            '¿Cuál es la función principal de la fileteadora en confección industrial?',
          imagen: '@/assets/actividad/imagen8.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Elaborar ojales rectos en camisas y chaquetas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Fijar botones planos sobre todo tipo de prendas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Sobrehilar, unir o pulir bordes textiles.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Realizar dobladillos invisibles en prendas formales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 19,
          texto:
            '¿Qué parámetro de calibración regula la distancia entre una puntada y la siguiente?',
          imagen: '@/assets/actividad/imagen9.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Presión del prensatelas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Longitud de puntada.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Altura del pedal.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Sistema de aguja.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },

        {
          id: 20,
          texto:
            '¿Qué información debe contener una ficha técnica de confección?',
          imagen: '@/assets/actividad/imagen10.png',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Materiales, medidas, maquinaria, operaciones, puntadas y acabados.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Horarios administrativos, nombres comerciales y ventas mensuales.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Fotografías promocionales, redes sociales y campañas de marca.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Costos personales, contratos laborales y datos bancarios.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia dominio técnico de la maquinaria y la tipología de prendas en los procesos de costura.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo relacionados con maquinaria y tipología de prendas.',
        },
      ],
      mensaje_final_aprobado:
        'Ha superado la actividad y demuestra sólidos conocimientos sobre maquinaria y tipología de prendas.',
      mensaje_final_reprobado:
        'No ha superado la actividad. Se recomienda revisar nuevamente el componente formativo e intentar de nuevo la actividad didáctica.',
    },
  }),
}
</script>
