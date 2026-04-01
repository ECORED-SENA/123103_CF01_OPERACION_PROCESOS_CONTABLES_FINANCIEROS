<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Fundamentos de contabilidad y registro de transacciones.',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> Evaluar el nivel de comprensión de los aprendices sobre los fundamentos de la contabilidad, la clasificación de soportes y el ciclo contable, así como su capacidad para registrar transacciones mediante el uso de la cuenta T y la aplicación de la partida doble, fortaleciendo la generación de información financiera confiable para la toma de decisiones organizacionales fundamentada en datos.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO.',
      preguntas: [
        {
          id: 1,
          texto: '¿Qué entiende por contabilidad?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es el arte de registrar únicamente las salidas de dinero o efectivo para evitar que la empresa entre en quiebra técnica o en crisis financiera',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Es un sistema de información que permite identificar, medir, clasificar y registrar las operaciones económicas para facilitar la toma de decisiones y el control',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Es una herramienta opcional y proporconal que se utiliza únicamente para el cálculo y pago de impuestos ante la administración tributaria',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Es el proceso de archivar facturas y documentos contables en orden cronológico para cumplir con las visitas de auditoría de la DIAN',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 2,
          texto:
            'Según el Decreto 2649 de 1993, el principio o norma técnica que establece que los hechos económicos deben ser reconocidos y registrados en el período en el cual ocurren, y no solamente cuando se recibe o paga el efectivo o su equivalente, se denomina:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Principio de Prudencia',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Norma de Valuación o Medición',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Principio de Continuidad',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Principio de Causación',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 3,
          texto: '¿Qué entiende por Plan Único de Cuentas (PUC)?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es un catálogo libre donde cada contador público asigna los números y nombres de las cuentas según su preferencia personal o institucional',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Es un listado de los precios de venta de los productos o artículos y servicios que ofrece una empresa al mercado para generar mayores ingresos',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Es una relación ordenada y clasificada de las cuentas que permite la uniformidad en el registro de las operaciones económicas, buscando transparencia y claridad',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Es un software contable automático que realiza el pago de impuestos sin necesidad de intervención humana',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 4,
          texto:
            '¿Por qué es fundamental que la contabilidad se rija por principios o normas técnicas?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Para que cada empresa pueda diseñar sus propios códigos y fórmulas según su conveniencia financiera',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Para garantizar que la información sea uniforme, comparable y transparente para todos los usuarios interesados',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Porque es un requisito secundario que solo aplica cuando la empresa decide solicitar un préstamo bancario',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Con el único fin de que los libros contables se vean organizados estéticamente ante una auditoría externa',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 5,
          texto:
            '¿Cómo se define el concepto de "Empresa" desde una perspectiva económica y contable?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es un grupo de personas o grupos de interés que se reúne exclusivamente para realizar actividades recreativas sin fines de lucro',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Es una organización dedicada a actividades industriales, mercantiles o de prestación de servicios con el fin de obtener un beneficio económico',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Es un edificio o estructura física donde se guardan mercancías, artículos o productos desarrollados para protegerlas del clima y otrs factores externos que puedan afectar su conservación',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Es cualquier contrato firmado de manera física o vitual en plataformas electrónicas como SECOP I o II, entre dos personas naturales o jurídicas para prestarse un favor personal',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 6,
          texto:
            '¿Qué se entiende por "Activo" dentro de la estructura financiera de una organización?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Son todas las obligaciones y deudas que la empresa ha contraído con terceros para poder operar un actividad económica, en el marco de la razón social',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Es el aporte inicial realizado por los socios o propietarios al momento de constituir legalmente la empresa, a través de los cuales, realizarán alistamiento e inicio de actividades',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Es un recurso controlado por la entidad como resultado de sucesos pasados, del cual se espera obtener beneficios económicos futuros',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Representa de manera única y exclusiva el dinero en efectivo que la empresa u organización tiene guardado en sus cajas de seguridad',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 7,
          texto:
            '¿Cómo se define el "Pasivo" dentro de la estructura financiera de una empresa?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Representa los aportes en dinero o en especie realizados por los dueños o socios para organización iniciar la operación de la actividad económica principal',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Es una obligación presente de la entidad, surgida a raíz de sucesos pasados, al vencimiento de la cual se espera desprenderse de recursos',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Son los bienes y derechos de propiedad de la empresa que tienen la capacidad de generar beneficios y riqueza en el futuro, en un periodo de cinco años',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Se refiere exclusivamente al valor de las ventas que la empresa espera realizar durante el próximo año fiscal, las cuales, fueron proyectadas desde la planeación estratégica',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 8,
          texto:
            '¿Qué se entiende por "Patrimonio" en el contexto de los estados financieros de una empresa?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es el conjunto de bienes y derechos que la empresa posee para su funcionamiento diario',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Representa el valor total de las ventas y servicios prestados por la entidad durante un año',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Es la parte residual de los activos de la entidad, una vez deducidos todos sus pasivos',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Se refiere únicamente al dinero en efectivo que los socios prometieron aportar pero que aún no han entregado',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 9,
          texto:
            '¿Qué son las "Cuentas Nominales" o de resultado y cuál es su principal característica?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Son cuentas o rubros permanentes que representan los bienes, deudas y el capital de la empresa, y su saldo se traslada de un año a otro',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Son cuentas que solo se utilizan para registrar los aportes de los socios o propietarios al momento de crear la empresa legalmente ante la Cámara de Comercio',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Son aquellas que registran los ingresos, gastos y costos de la entidad, y se cierran al final de cada ejercicio contable para determinar la utilidad o pérdida',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Son los registros que se llevan únicamente de forma extracontable y extemporánea para controlar los activos que no pertenecen a la empresa',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 10,
          texto:
            '¿Cómo se clasifican las "Cuentas Nominales" o de resultado dentro del sistema contable?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Se clasifican en Ingresos, Gastos y Costos (de ventas y de producción)',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Se clasifican en Activos, Pasivos y Patrimonio, que reflejan la situación financiera y real de una empresa',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Se clasifican en Cuentas de Orden Deudoras y Cuentas de Orden Acreedoras',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Se clasifican únicamente en Cuentas de Control y Cuentas de Detalle, dependiendo del tipo, tamaño y sector de la empresa',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 11,
          texto:
            '¿Cuál es la diferencia principal entre un "Deudor" y un "Acreedor" en el contexto contable?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Un deudor es quien debe dinero a la empresa, mientras que un acreedor es la persona o entidad a quien la empresa le debe dinero',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Un deudor es el dueño de la empresa y el acreedor es el banco que le otorga los préstamos personales para brindar solución a una contingencia',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Los deudores son siempre empleados de la organización, mientras que los acreedores son únicamente los clientes que compran de contado',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'No existe diferencia técnica, ambos términos se utilizan indistintamente para referirse a los socios de la compañía, lo que intesa son su participación determinada como aporte',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 12,
          texto:
            '¿En qué consiste la “Partida Doble” en el registro de las operaciones contables?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es un sistema que consiste en registrar dos veces la misma transacción en diferentes libros para evitar que la información se pierda',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Es la técnica especializada de anotar únicamente las deudas que la empresa tiene con dos o más bancos al mismo tiempo, que se encuentren en la misma ciudad',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Es el método que establece que en cada operación debe haber, como mínimo, un elemento deudor (Debe) y uno acreedor (Haber) que sumen valores iguales',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Se refiere a la obligación de tener dos contadores distintos revisando la misma cuenta para evitar errores humanos y realizar mayor seguimiento y control a cada registro contable',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 13,
          texto: '¿Cuál de los siguientes elementos pertenece al activo?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Cuentas por pagar',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Capital social',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Caja',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Préstamos bancarios',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },

        {
          id: 14,
          texto:
            '¿Cuál de las siguientes situaciones representa un pasivo para la empresa?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un préstamo pendiente con una entidad financiera',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Dinero en banco disponible para retiro de la empresa',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Mercancía para la venta directa o entregar en consignación',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Equipos de oficina para la operación de la empresa',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 15,
          texto: 'El patrimonio de una empresa aumenta cuando:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Se adquiere una deuda',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Se generan utilidades',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Se pagan obligaciones',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Se disminuyen los activos',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 16,
          texto: '¿Cuál de los siguientes es un ejemplo de pasivo?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Inventarios',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Clientes',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Proveedores',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Equipos',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 17,
          texto:
            'Si una empresa tiene activos por $100.000 y pasivos por $40.000, su patrimonio es:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: '$140.000',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: '$40.000',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: '$100.000',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: '$60.000',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 18,
          texto: 'Cuando una empresa paga una deuda, ¿qué ocurre?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Disminuye el activo y el pasivo',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Aumenta el activo y el pasivo',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Aumenta el patrimonio y el gasto',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'No hay ningún cambio, sin novedades',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 19,
          texto: 'Las cuentas del activo se caracterizan por:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentar en el haber y disminuir en el debe',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Aumentar en el debe y disminuir en el haber',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Aumentar y disminuir únicamente en el debe',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'No tener ningún movimiento contable',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
        {
          id: 20,
          texto:
            'Las cuentas de pasivo y patrimonio presentan el siguiente comportamiento:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentan en el debe y disminuyen en el haber',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Solo aumentan en el debe, por su naturaleza',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'No disminuyen nunca, permanecen estáticas',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Aumentan en el haber y disminuyen en el debe',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Su respuesta es correcta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta es incorrecta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
