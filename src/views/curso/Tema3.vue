<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(:subTitulo="'3. Métodos básicos de acumulación de costos'")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .row.mb-5
      .col-lg-5
        figure
          img(src="@/assets/curso/tema3/1.png", data-aos="zoom-in")
      .col-lg-7.bg-color-4.p-5
        p(data-aos="fade-left").mb-0 Los <b>métodos básicos de acumulación de costos</b>, se refiere a los procedimientos y técnicas utilizadas por las empresas para asignar o distribuir los costos a los productos o servicios que producen. Estos métodos son necesarios en la contabilidad de costos, dado que permiten determinar el costo de producción de cada unidad, ayudando a tomar decisiones sobre precios, márgenes de ganancia y eficiencia operativa. Los métodos más comunes incluyen:


    #t_3_1.titulo-segundo(data-aos="flip-up")
      h2 #[span 3.1] Costeo ABC (<em>Activity Base Costing</em>)

    p.mb-5 El Costeo Basado en Actividades o ABC (<em>Activity-Based Costing</em>), es un método de acumulación de costos que asigna los costos indirectos a los productos y servicios, en función de las actividades que generan esos costos. A diferencia de otros métodos tradicionales de costeo, que asignan los costos indirectos de manera general o, según volumen, el ABC se enfoca en identificar y asignar los costos a las actividades que realmente consumen recursos dentro de la empresa.

    .titulo-figura.mb-4
      h5 Tabla 2. 
      span Características, ventajas y desventajas de los costos ABC.

    .tabla-a.color-terciario.mb-5 
      table
        thead
          tr
            th.bg-color-5.text-center Características
            th.bg-color-5.text-center Ventajas
            th.bg-color-5.text-center Desventajas
        tbody
          tr.bg-color-6
            td <b>Identificación de actividades</b>: en primer lugar, se identifican todas las actividades realizadas en la empresa, las cuales generan costos, como la preparación de materiales, la inspección de calidad, la distribución, entre otras.
            td <b>Mayor precisión en la asignación de costos:</b> el costeo ABC, ayuda en la asignación de los costos indirectos, de manera más precisa, porque se basa en las actividades que realmente generan el costo.
            td <b>Complejidad:</b> requiere un análisis detallado de las actividades y un sistema de medición que puede ser más complejo y costoso de implementar.
            
          tr.bg-color-6
            td <b>Asignación de costos a las actividades:</b> luego, los costos indirectos (como la electricidad, la depreciación de equipos, etc.), se asignan a cada una de estas actividades, en función de su uso de recursos.
            td <b>Mejor toma de decisiones:</b> al tener una visión más clara de qué actividades son más costosas, la empresa puede identificar áreas de mejora y optimizar sus procesos.
            td <b>Tiempo y recursos:</b> es más costoso y consume más tiempo que los métodos tradicionales de asignación de costos.
           
          tr.bg-color-6
            td <b>Determinación de los costos de las actividades:</b> para cada actividad identificada, se mide el costo asociado, generalmente mediante cost drivers (factores que impulsan el costo de la actividad). Esto puede ser la cantidad de horas de mano de obra, la cantidad de unidades producidas, el número de órdenes de compra, etc.
            td <b>Claridad en la rentabilidad de productos o servicios:</b> permite identificar qué productos o servicios son más rentables y cuáles son menos rentables, lo que puede influir en decisiones sobre precios o discontinuación de productos.
            td 
             
          tr.bg-color-6
            td <b>Asignación a los productos:</b> finalmente, los costos de cada actividad se distribuyen entre los productos o servicios, según el nivel de actividad que cada uno consuma.
            td 
            td 
    
    p.mb-5 A través de un ejemplo práctico, se ilustrará cómo aplicar el costeo ABC, facilitando la comprensión de su impacto en la toma de decisiones y en la rentabilidad empresarial.

    .bg-full-width.bg-color-2
      .px-4.px-md-5.pb-md-3.pt-md-5

        h2 Ejemplo de asignación de costos ABC
        p La empresa fabrica dos productos: <b>A y B</b>, y asigna costos, basados en dos actividades principales: <b>inspección y empaquetado</b>.

        .titulo-figura.mb-4
          h5 Tabla 3. 
          span Costos de actividades y <em>cost drivers</em>
        .row.mb-5
          .col-lg-11
            .tabla-a.color-terciario.mb-5 
              table
                thead
                  tr
                    th.bg-color-5 Actividad
                    th.bg-color-5 Costo total ($)
                    th.bg-color-5 <em>Cost Driver</em>
                    th.bg-color-5 Detalle
                tbody
                  tr.bg-color-6
                    td Inspección
                    td $5,000
                    td 1 inspección cada 100 unidades
                    td 15 inspecciones (5 para A y 10 para B)
                    
                  tr.bg-color-6
                    td Empaque
                    td $3,000
                    td 1 lote por cada 200 unidades
                    td 8 lotes (3 para A y 5 para B)

        h2 Cálculo de costos por actividad

        ul.lista-ul
          li.text-bold 
            i.lista-ul__vineta
            | Inspección:
          li
            ul
              li.mb-0
                i.lista-ul__vineta
                | Total de inspecciones: 15
              li.mb-0
                i.lista-ul__vineta
                | Costo por inspección: $5,000 ÷ 15 = $333.33
              li.mb-0
                i.lista-ul__vineta
                | Producto A (5 inspecciones): 5×333.33=1,666.675 \times 333.33 = 1,666.675×333.33=1,666.67
              li.mb-0
                i.lista-ul__vineta
                | Producto B (10 inspecciones): 10×333.33=3,333.3310 \times 333.33 = 3,333.3310×333.33=3,333.33
        
        ul.lista-ul
          li.text-bold 
            i.lista-ul__vineta
            | Empaque:
          li
            ul
              li.mb-0
                i.lista-ul__vineta
                | Total de lotes: 8
              li.mb-0
                i.lista-ul__vineta
                | Costo por lote: $3,000 ÷ 8 = $375
              li.mb-0
                i.lista-ul__vineta
                | Producto A (3 lotes): 3×375=1,1253 \times 375 = 1,1253×375=1,125
              li.mb-0
                i.lista-ul__vineta
                | Producto B (5 lotes): 5×375=1,8755 \times 375 = 1,8755×375=1,875

        .titulo-figura.mb-4
          h5 Tabla 4. 
          span Distribución total de costos por producto
        
        .row 
          .col-lg-8
            .tabla-a.color-terciario.mb-5 
              table
                thead
                  tr
                    th.bg-color-5 Producto
                    th.bg-color-5 Costo de inspección ($)
                    th.bg-color-5 Costo de empaquetado ($)
                    th.bg-color-5 Total ($)
                tbody
                  tr.bg-color-6
                    td Producto A
                    td 1,666.67
                    td 1,125
                    td 2,791.67
                    
                  tr.bg-color-6
                    td Producto B
                    td 3,333.33
                    td 1,875
                    td 5,208.33
        
        p.text-bold Resumen:

        p ●	<b>Producto A:</b> Total de costos = <b>$2,791.67</b>
        p ●	<b>Producto B:</b> Total de costos = <b>$5,208.33</b>

        p Este ejemplo ilustra cómo el método de <b>Costeo Basado en Actividades (ABC)</b> asigna los costos de manera más precisa al utilizar <em>cost drivers</em>, para actividades específicas.
 
          
    #t_3_2.titulo-segundo(data-aos="flip-up").mt-5
      h2 #[span 3.2] Costeo por órdenes de trabajo (o por órdenes específicas)

    p(data-aos="fade-left").mb-4 Este método se utiliza cuando la producción de bienes o servicios es por lotes o, según pedidos específicos de los clientes. Se acumulan los costos directos (materiales, mano de obra, etc.) y los costos indirectos (como la depreciación de maquinaria o energía), para cada orden de trabajo, de manera individual. Es común en industrias como la fabricación a medida, construcción o proyectos específicos.

    .row.justify-content-center.align-items-stretch.mb-5
      .col-lg-6.mb-4(data-aos="zoom-in-up")
        .custom-image-card-2.h-100
          img.custom-image-card__image(src="@/assets/curso/tema3/2.png" alt="")
          .custom-image-card__text.p-4
            h5.mb-2.text-center Ventajas	
            p.mb-0 Facilita el cálculo de costos específicos por cada orden, lo que es útil para personalizar el precio, según las características de cada trabajo.
      .col-lg-6.mb-4(data-aos="zoom-in-down")
        .custom-image-card-2.h-100
          img.custom-image-card__image(src="@/assets/curso/tema3/3.png" alt="")
          .custom-image-card__text.p-4
            h5.mb-2.text-center Desventajas		
            p.mb-0 Requiere una buena organización para asignar correctamente, los costos a cada orden, lo que puede ser costoso y complejo.
    
    p.mb-5 A través de un ejemplo práctico, se mostrará cómo se asignan materiales, mano de obra y costos indirectos, a una orden de trabajo, lo que contribuye a una gestión más precisa y a una mejor toma de decisiones en la producción.

    .bg-full-width.bg-color-2
      .px-4.px-md-5.pb-md-3.pt-md-5

        h2 Ejemplo de costeo por órdenes de trabajo
        p En este ejemplo, una empresa produce <b>10 mesas</b> y <b>15 sillas</b>, acumulando los costos en órdenes de trabajo específicas.

        .titulo-figura.mb-4
          h5 Tabla 5. 
          span Costos directos
        .row.mb-5
          .col-lg-7
            .tabla-a.color-terciario.mb-5 
              table
                thead
                  tr
                    th.bg-color-5 Concepto
                    th.bg-color-5 Cálculo
                    th.bg-color-5 Costo total ($)
                tbody
                  tr.bg-color-6
                    td(rowspan="2") <b>Mesas</b>
                    td Materiales: 10 x $100
                    td $1,000
                  tr.bg-color-6
                    td Mano de obra: 10 x $50
                    td $500
                  tr.bg-color-6
                    td(rowspan="2") <b>Sillas</b>
                    td Materiales: 15 x $50
                    td $750
                  tr.bg-color-6
                    td Mano de obra: 15 x $30
                    td $450

        h2 Costos indirectos

        p Los costos indirectos de $1,000 se asignan en función de las horas de trabajo.

        ul.lista-ul
          li
            i.lista-ul__vineta
            | Total de horas trabajadas: <b>100 horas</b>
          li
            ul
              li.mb-0
                i.lista-ul__vineta
                | Mesas: <b>60 horas</b> → Proporción: 60/100=0.6060 / 100 = 0.6060/100=0.60
              li.mb-0
                i.lista-ul__vineta
                | Sillas: <b>40 horas</b> → Proporción: 40/100=0.4040 / 100 = 0.4040/100=0.40

        .titulo-figura.mb-4
          h5 Tabla 6. 
          span Costos indirectos
        
        .row 
          .col-lg-10
            .tabla-a.color-terciario.mb-5 
              table
                thead
                  tr
                    th.bg-color-5 Orden
                    th.bg-color-5 Proporción de horas
                    th.bg-color-5 Asignación costos indirectos ($)
                tbody
                  tr.bg-color-6
                    td <b>Mesas</b>
                    td 0.60
                    td 0.60×1,000=6000.60 \times 1,000 = 6000.60×1,000=600
                    
                    
                  tr.bg-color-6
                    td <b>Sillas</b>
                    td 0.40
                    td 0.40×1,000=4000.40 \times 1,000 = 4000.40×1,000=400

        .titulo-figura.mb-4
          h5 Tabla 7. 
          span Cálculo del costo total por orden
        
        .row 
          .col-lg-10
            .tabla-a.color-terciario.mb-5 
              table
                thead
                  tr
                    th.bg-color-5 Orden
                    th.bg-color-5 Costos directos ($)
                    th.bg-color-5 Costos indirectos ($)
                    th.bg-color-5 Costo total ($)
                tbody
                  tr.bg-color-6
                    td <b>Orden 1 (mesas)</b>
                    td 1,500
                    td 600
                    td 2,100
                    
                    
                  tr.bg-color-6
                    td <b>Orden 2 (sillas)</b>
                    td 1,200
                    td 400
                    td 1,600         
        
        p.text-bold Resultado final:

        p.text-bold ●	Orden 1 (mesas): $2,100
        p.text-bold ●	Orden 2 (sillas): $1,600

        p Este ejemplo refleja cómo se asignan los costos directos e indirectos en el <b>costeo por órdenes de trabajo</b>, permitiendo un control preciso sobre cada producción.

    p.mt-5 Los métodos de acumulación de costos, son sistemas que permiten registrar y asignar los costos incurridos en la producción de bienes o servicios. Dependiendo de las características del proceso productivo, se pueden aplicar distintos métodos, como el costeo por órdenes de trabajo, ideal para productos personalizados, o el costeo por procesos, utilizado en producciones masivas y estandarizadas. 
    
    .bg-full-width.bg-color-9
      .px-4.px-md-5.pb-md-3.pt-md-5
        .row.mb-5.align-items-center
          .col-lg-7
            h2 Métodos de acumulación de costos
            p Se invita a analizar los diferentes <b>métodos de acumulación de costos</b>, herramientas esenciales para la gestión eficiente de recursos en proyectos o empresas. El documento expone cómo el costeo por procesos, el costeo variable, el costeo absorbente y el costeo estándar, ofrecen enfoques adaptados a distintas necesidades de producción y control financiero. A través de ejemplos prácticos, se presentan las ventajas, desventajas y su impacto en la planificación empresarial, facilitando su comprensión y aplicación en contextos reales. Este análisis permitirá profundizar en las bases del control de costos y la optimización de recursos.

            .bg-color-white.shadow-soft.py-3.px-lg-4
              .row.justify-content-around.align-items-center
                .col-md-auto
                  img(src="@/assets/template/bg-icono-pdf.svg", style="width: 45px;")
                .col
                  .row.justify-content-between.align-items-center
                    .col.mb-3.mb-sm-0
                      p.text-small <b>Anexo.</b> Métodos de acumulación de costos
                    .col-sm-auto
                      a.boton.color-acento-botones.texto-blanco(:href="obtenerLink('/downloads/prueba.pdf')" target="_blank")
                        span.text-small Descargar
                        i.fas.fa-arrow-right
          .col-lg-5
            figure
              img(src='@/assets/curso/tema3/4.png', alt='')
      

    .bg-full-width.border-top.color-primario
      .p-4.p-md-5
        h2(data-aos="fade-left") MATERIAL COMPLEMENTARIO
        .row.material-complementario
          .col-12.col-md-6.col-lg-7
            p Los invitamos a explorar el material complementario de este curso, en esta sección encontrará recursos que le permitirán profundizar  y enriquecer su aprendizaje en los temas tratados en esta unidad.

            //- Referencia con enlace 
            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://www.revistasice.com/index.php/CICE/article/download/6031/6031" target="_blank" rel="noopener noreferrer") De Castro Emilio Cerdá, F. J. A. L. M. (s/f). Las energías renovables en el ámbito internacional. Revistasice.com. 

            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://natura.org.co/que-es-agricultura-sostenible-y-como-se-relaciona-con-el-monitoreo-climatico/" target="_blank" rel="noopener noreferrer") Natura, F. (2024, junio 6). ¿Qué es agricultura sostenible y cómo se relaciona con el monitoreo climático? Fundación Natura Colombia. 

            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://www.revistaecosistemas.net/index.php/ecosistemas/article/view/614" target="_blank" rel="noopener noreferrer") Artaraz, M. (2002). Teoría de las tres dimensiones de desarrollo sostenible: . Ecosistemas, 11(2). 

            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://elibro.net/es/ereader/tecnologicadeloriente/62332?page=170" target="_blank" rel="noopener noreferrer") Fernández García, R. (2013). La dimensión económica del desarrollo sostenible: ( ed.). ECU.

            p.d-flex.my-4
              img.me-3(src='@/assets/componentes/link.svg' :style="{'max-width':'16px'}")
              a(href="https://elibro.net/es/lc/tecnologicadeloriente/titulos/274611" target="_blank" rel="noopener noreferrer") De Castro Emilio Cerdá, F. J. A. L. M. (s/f). Las energías renovables en el ámbito internacional. Revistasice.com. 

            //- Referencia sin enlace 
            p.d-flex.my-4
              img.me-3(src='@/assets/template/book.svg' :style="{'max-width':'16px'}")
              span Cerdos criollos colombianos y agricultura sostenible. 

            p.d-flex.my-4
              img.me-3(src='@/assets/template/book.svg' :style="{'max-width':'16px'}")
              span De Janeiro, R. (1992). La declaración del Río sobre el Medio Ambiente y el Desarrollo. Río de Janeiro República Federativa del Brasil., aprobada en Estocolmo el, 16.

            //- Referencia de youtube 
            p.d-flex.my-4
              img.me-3(src='@/assets/template/icono-yt.svg' :style="{'max-width':'16px'}")
              a(href="https://youtu.be/hlpTZbikazw?si=XGBJEV3L-9pTa-Gc" target="_blank" rel="noopener noreferrer") Empresas innovadoras.

            p.d-flex.my-4
              img.me-3(src='@/assets/template/icono-yt.svg' :style="{'max-width':'16px'}")
              a(href="https://youtu.be/Kh5lpqxTw5M?si=NN1qB14TbGN9TxiU" target="_blank" rel="noopener noreferrer") Google, Microsoft y tesla, el verdadero rey de la inteligencia artificial.

            p.d-flex.my-4
              img.me-3(src='@/assets/template/icono-yt.svg' :style="{'max-width':'16px'}")
              a(href="https://youtu.be/QKLjwCMyv3M?si=uAWhO9tnyghljaJg" target="_blank" rel="noopener noreferrer") Innovación y sostenibilidad.
              
          .col-12.col-md-6.col-lg-3.offset-lg-1
            figure
              img(src='@/assets/componentes/material-complementario.svg', alt='')

</template>

<script>
export default {
  name: 'Tema3',
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
}
</script>
