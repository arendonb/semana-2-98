<template>
  <footer
    class="page-footer text-black pt-4"
    style="background-color: lightgray"
  >
    <!-- Footer Text -->
    <div class="container-fluid text-center text-md-left">
      <!-- Grid row -->
      <div class="row">
        <!-- Grid column -->
        <div class="col-md-6 mt-md-0 mt-3">
          <!-- Content -->
          <h5 class="text-uppercase font-weight-bold">Motivación</h5>
          <br />
          <p>
            Esta página fue creada con la motivación de aprender a trabajar con
            Bootstrap, Vue Cli y el manejo de APIs.<br />
            <br />

            <a
              class="navbar-brand"
              href="https://github.com/arendonb/semana-2-98"
              target="_blank"
            >
              <img
                src="https://www.flaticon.es/svg/vstatic/svg/25/25231.svg?token=exp=1607611344~hmac=40f687c7b38016da882b5fa873454efc"
                width="40"
                height="40"
                alt=" "
                loading="lazy "
              />
              GitHub</a
            >
            <br />
          </p>
        </div>
        <!-- Grid column -->

        <hr class="clearfix w-100 d-md-none pb-3" />

        <!-- Grid column -->
        <div class="col-md-6 mb-md-0 mb-3">
          <!-- Content -->
          <h5 class="text-uppercase font-weight-bold">Contacto</h5>
          <br />
          <p>
            Santiago Andres Millan Pardo

            <small class="text-muted">
              Bogotá - santiagomillanpardo@gmail.com</small
            >
            <br />
            <br />
            Cristhian Daniel Díaz Salazar

            <small class="text-muted"> Pereira - crdadiaz@utp.edu.co </small>
            <br />
            <br />
            Miguel Enrique Marquez Aldana

            <small class="text-muted">
              Bogotá - miguelmarquez.99@gmail.com</small
            >
            <br />
            <br />
            Diego Luis Soto Mendoza

            <small class="text-muted">
              Villavicencio - diegoluissotomendoza@gmail.com</small
            >
            <br />
            <br />
            Alejandro Rendón Blandon

            <small class="text-muted"> Medellín - arendonb@gmail.com </small>
            <br />
            <br />
          </p>
        </div>
        <!-- Grid column -->
      </div>
      <!-- Grid row -->
    </div>
    <!-- Footer Text -->

    <!-- Copyright -->
    <div
      class="footer-copyright text-center text-black py-1"
      style="background-color: lightgray"
    >
      <img
        src="https://img.icons8.com/ios/50/000000/98.png"
        width="35"
        height="35
            "
        class="d-inline-block align-center"
        alt=""
        loading="lazy "
      />
      <br />
      © 2020 Copyright: DAD
    </div>
    <!-- Copyright -->
  </footer>
</template>

<script>
export default {
  name: "PageFooter",
};
</script>

<style scoped>
a {
  color: black;
}

a:visited {
  color: Black;
}

a:hover {
  color: blue;
}
</style>