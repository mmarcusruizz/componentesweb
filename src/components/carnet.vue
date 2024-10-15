<script>
export default {
  name: 'carnet',
  data() {
    return {
      //data que se renderiza en el template html 
      nombres: 'ELON REEVE',
      apellidos: 'MUSK',
      sexo: 'M',
      nacionalidad: 'SUDAFRICANO',
      numeroDeDocumento: '222.222.222',
      run: '22.222.222-2',
      fechaDeNacimiento: '28 JUN 1971',
      fechaDeEmision: '01 ENE 2025',
      fechaDeVencimiento: '01 ENE 2030',
      firmaDelTitular: 'XXX A-12',
    }
  },
}
</script>
<template>
  <body>
    <div class="carnet">
      <aside>
        <div>
          <span>CEDULA DE INDENTIDAD</span>
          <img width="40" src="/src/assets/img/chile_bandera.png" alt="" />
        </div>

        <img src="/src/assets/img/foto_elon.jpg" alt="" />
        <p>RUN {{ run }}</p>
      </aside>

      <main>
        <header>
          <p>REPUBLICA DE CHILE</p>
          <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
        </header>
        <section>
          <article>
            <header>APELLIDOS</header>
            <span>{{ apellidos }}</span>
          </article>
          <article>
            <header>NOMBRES</header>
            <span>{{ nombres }}</span>
          </article>

          <div class="grid-2-colums">
            <article>
              <header>NACIONALIDAD</header>
              <span>{{ nacionalidad }}</span>
            </article>
            <article>
              <header>SEXO</header>
              <span>{{ sexo }}</span>
            </article>
          </div>
          <div class="grid-2-colums">
            <article>
              <header>FECHA DE NACIMIENTO</header>
              <span>{{ fechaDeNacimiento }} </span>
            </article>
            <article>
              <header>NÙMERO DOCUMENTO</header>
              <span>{{ numeroDeDocumento }}</span>
            </article>
          </div>
          <div class="grid-2-colums">
            <article>
              <header>FECHA DE EMISIÒN</header>
              <span>{{ fechaDeEmision }}</span>
            </article>
            <article>
              <header>FECHA DE VENCIMIENTO</header>
              <span>{{ fechaDeVencimiento }}</span>
            </article>
          </div>
          <article>
            <header>FIRMA DEL TITULAR</header>
            <span>{{ firmaDelTitular }}</span>
          </article>
        </section>
      </main>
    </div>
  </body>
</template>
