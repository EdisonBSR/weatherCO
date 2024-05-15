<template>
  <div>
    <b-form @submit="onSubmit">
      <div id="containerCard">
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top
          tag="article" style="max-width: 20rem;" class="mb-2">
          <b-card-text>
            Pondria en esta parte todo lo relacionado con los datos del clima
          </b-card-text>
          <b-button type="submit" variant="primary">Conocer Clima</b-button>
          <b-form-select v-model="selectedCity1" :options="options"></b-form-select>
        </b-card>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top
          tag="article" style="max-width: 20rem;" class="mb-2">
          <b-card-text>
            Pondria en esta parte todo lo relacionado con los datos del clima
          </b-card-text>
          <b-button href="#" variant="primary">Conocer Clima</b-button>
          <b-form-select v-model="selectedCity2" :options="options"></b-form-select>
        </b-card>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top
          tag="article" style="max-width: 20rem;" class="mb-2">
          <b-card-text>
            Pondria en esta parte todo lo relacionado con los datos del clima
          </b-card-text>
          <b-button href="#" variant="primary">Conocer Clima</b-button>
          <b-form-select v-model="selectedCity3" :options="options"></b-form-select>
        </b-card>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top
          tag="article" style="max-width: 20rem;" class="mb-2">
          <b-card-text>
            Pondria en esta parte todo lo relacionado con los datos del clima
          </b-card-text>
          <b-button href="#" variant="primary">Conocer Clima</b-button>
          <b-form-select v-model="selectedCity4" :options="options"></b-form-select>
        </b-card>
        <b-card title="Card Title" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top
          tag="article" style="max-width: 20rem;" class="mb-2">
          <b-card-text>
            Pondria en esta parte todo lo relacionado con los datos del clima
          </b-card-text>
          <b-button href="#" variant="primary">Conocer Clima</b-button>
          <b-form-select v-model="selectedCity5" :options="options"></b-form-select>
        </b-card>
      </div>
      <b-button type="submit" variant="success">Clima</b-button>
    </b-form>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    onSubmit(event) {
      event.preventDefault()
      alert("hola")
    }
  },
  data() {
    return {
      selectedCity1: null,
      selectedCity2: null,
      selectedCity3: null,
      selectedCity4: null,
      selectedCity5: null,
      options: [
        { value: null, text: 'Seleccione una ciudad' },
        { value: 'Bogota', text: 'Bogota' },
        { value: 'Cali', text: 'Cali' },
        { value: 'Villavicencio', text: 'Villavicencio' },
        { value: 'Popayan', text: 'Popayan' },
        { value: 'Medellin', text: 'Medellin' },
        { value: 'Cartagena', text: 'Cartagena' },
        { value: 'Barranquilla', text: 'Barranquilla' }
      ]
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#containerCard {
  display: flex;
  flex-direction: row;
  justify-items: space-between;
}

.mb-2 {
  margin: 10px;
}
</style>
