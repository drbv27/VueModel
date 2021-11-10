<template>
  <form>
    <input
      type="text"
      class="form-control my-2"
      placeholder="Ingrese nombre"
      v-model="tarea.nombre"
    />
    <div class="form-check form-check-inline">
      <input
        type="checkbox"
        id="check-1"
        class="form-check-input"
        v-model="tarea.categorias"
        value="javascript"
      />
      <label for="check-1" class="form-check-label">Javascript</label>
    </div>
    <div class="form-check form-check-inline">
      <input
        type="checkbox"
        id="check-2"
        class="form-check-input"
        v-model="tarea.categorias"
        value="node js"
      />
      <label for="check-2" class="form-check-label">Node.js</label>
    </div>
    <div class="mt-2">
      <div class="form-check form-check-inline">
        <input
          type="radio"
          id="radio-1"
          class="form-check-input"
          value="urgente"
          v-model="tarea.estado"
        />
        <label for="radio-1" class="form-check-label">Urgente</label>
      </div>
      <div class="form-check form-check-inline">
        <input
          type="radio"
          id="radio-2"
          class="form-check-input"
          value="relax"
          v-model="tarea.estado"
        />
        <label for="radio-2" class="form-check-label">Relax</label>
      </div>
    </div>
    <div class="mt-2">
      <input
        class="form-control"
        type="number"
        name=""
        id=""
        v-model="tarea.numero"
      />
    </div>
  </form>
  <hr />
  <p>{{ tarea }}</p>
</template>

<script>
export default {
  name: "Home",
  components: {},
  data() {
    return {
      tarea: {
        nombre: "",
        categorias: [],
        estado: "",
        numero: 0,
      },
    };
  },
};
</script>
