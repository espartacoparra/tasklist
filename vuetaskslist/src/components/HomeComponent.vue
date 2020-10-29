<template>
  <div id="home-component">
    <div class="container">
      <div class="row">
        <div class="col-8 task-list">
          <b-card
            bg-variant="danger"
            text-variant="white"
            header="Pending Tasks"
            class="text-center mt-2"
          >
            <b-card-text> </b-card-text>
          </b-card>
        </div>
        <div class="col-4 form">
          <div>
            <b-form>
              <label class="sr-only" for="inline-form-input-name">Name</label>
              <b-input
                v-model="form.name"
                id="inline-form-input-name"
                class="mb-2 mr-sm-2 mb-sm-0"
                placeholder="Jane Doe"
              ></b-input>

              <label class="sr-only" for="inline-form-input-username"
                >Username</label
              >
              <b-input-group prepend="@" class="mb-2 mr-sm-2 mb-sm-0">
                <b-input
                  id="inline-form-input-username"
                  placeholder="Username"
                ></b-input>
              </b-input-group>

              <b-form-checkbox class="mb-2 mr-sm-2 mb-sm-0"
                >Remember me</b-form-checkbox
              >

              <b-button variant="primary">Save</b-button>
            </b-form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeComponent",
  props: {
    msg: String,
  },
  data() {
    return {
      form: {},
    };
  },
};
</script>
<style scoped>
.task-list {
  background-color: aquamarine;
}
.form {
  background-color: gray;
}
</style>
