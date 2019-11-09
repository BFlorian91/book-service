<template>
  <section id="authors" class="my-5 text-center">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="info-header mb-5">
            <h1 class="text-primary pb-3">Meet The Authors</h1>
            <p
              class="lead"
            >Lorem ipsum dolor sit amet consectetur adipisicing elit. Qui, praesentium!</p>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-3 col-md-6" v-for="(user, index) in users" :key="index">
          <div class="card">
            <div class="card-body">
              <img
                src="@/assets/img/me.jpeg"
                alt="me"
                class="img-fluid rounded-circle w-50 mb-3"
              />
              <h3>{{ user.name }}</h3>
              <h5 class="job">{{ user.job }}</h5>
              <p>
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptas unde placeat voluptatem voluptate expedita magni,
                modi.
              </p>
              <div class="d-flex justify-content-center">
                <div class="p-4">
                  <a href="https://facebook.com">
                    <i class="fab fa-facebook"></i>
                  </a>
                </div>
                <div class="p-4">
                  <a href="https://twitter.com">
                    <i class="fab fa-twitter"></i>
                  </a>
                </div>
                <div class="p-4">
                  <a href="https://instagram.com">
                    <i class="fab fa-instagram"></i>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      users: [
        { name: "Florian Beaumont", job: "CEO", photo: "person1.jpg" },
        { name: "Florian Beaumont", job: "Lead-developer", photo: "@/assets/img/Designer.jpg" },
        { name: "Florian Beaumont", job: "Front-developer", photo: "@/assets/img/Lead.jpg" },
        { name: "Florian Beaumont", job: "Designer", photo: "@/assets/img/CEO.jpg" },
      ]
    }
  }
};
</script>

<style>
</style>