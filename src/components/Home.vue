<template>
  <div class="py-5"></div>
  <div class="p">
    <h1 class="blue-text fw-bold Montserrat pb-1">Bringing Life To Film</h1>
  </div>

  <div class="row justify-content-lg-evenly">
    <div class="col-sm"></div>

    <div class="col-md-6">
      <div
        id="carouselExampleControls"
        class="carousel slide"
        data-bs-ride="carousel"
      >
        <div class="carousel-inner">
          <div class="carousel-item active">
            <img
              src="../assets/egphotos/IMG_3617.jpeg"
              class="d-block w-100 rounded"
              alt="..."
            />
          </div>
          <div class="carousel-item">
            <img
              src="../assets/egphotos/IMG_3618.jpeg"
              class="d-block w-100 rounded"
              alt="..."
            />
          </div>
        </div>
        <button
          class="carousel-control-prev"
          type="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button
          class="carousel-control-next"
          type="button"
          data-bs-target="#carouselExampleControls"
          data-bs-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
    </div>

    <div class="col-sm"></div>
  </div>
  <!-- Info Section -->
  <div class="py-5"></div>
  <div>
    <p>
      <span
        >{{ name }} is a fremantle based photography and film business. We
        specialize in catering and providing new cinomatic expirence for your
        uniuqe events.</span
      >
    </p>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      name: "name",
    };
  },
};
</script>

<style>
#app {
  text-align: center;
}
</style>
