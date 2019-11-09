<template>
  <section id="contact" class="bg-light py-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-9">
          <h3>Get In Touch</h3>
          <p
            class="lead"
          >Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptates cum minus maiores corporis iusto sequi optio sit cumque. Recusandae quod odio magnam officia molestiae neque nostrum ipsa tempora blanditiis dignissimos!</p>
          <form>
            <div
              class="input-group input-group-lg mb-3"
              v-for="(item, index) in items"
              :key="index"
            >
              <div class="input-group-prepend">
                <span class="input-group-text">
                  <i :class="item.icon"></i>
                </span>
              </div>
              <input type="text" class="form-control" :placeholder="item.name" />
            </div>
            <div class="input-group input-group-lg mb-3">
              <div class="input-group-prepend">
                <span class="input-group-text">
                  <i class="fas fa-pencil-alt"></i>
                </span>
              </div>
              <textarea type="text" class="form-control" placeholder="Text" rows="5" />
            </div>
            <input type="submit" value="Submit" class="btn btn-primary btn-block btn-lg" />
          </form>
        </div>
        <div class="col-lg-3 align-self-center">
          <img src="@/assets/img/mlogo.png" alt="logo" class="img-fluid" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { name: "Name", icon: "fa fa-user" },
        { name: "Email", icon: "fas fa-envelope-open-text" }
      ]
    };
  }
};
</script>

<style>
</style>