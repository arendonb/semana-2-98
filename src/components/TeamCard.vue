<template>
  <div  class="card text-black bg-light">
    <div class="d-flex justify-content-center p-3">
      <img v-bind:src="member.image" alt="Fotografia del equipo" />
    </div>
    <div class="card-body" style="height: 400px">
      <h5 class="card-title" style="text-align: center">{{ member.nombre }}</h5>
      <p class="card-text" style="text-align: center">
        <small class="text-muted"
          ><span>Código: </span> {{ member.codigo }}</small
        >
      </p>
      <p class="card-text" style="text-align: justify">
        {{ member.descripcion }}
      </p>
    </div>
    <div class="card-footer">
      <p style="text-align: center">
        <b>{{ member.rol }}</b>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "TeamCard",
  props: ["member"],
};
</script>

<style scoped>
img {
  height: 150px;
  width: 150px;
  border-radius: 50%;
}
</style>
