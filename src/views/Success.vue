<template>
  <div>
    <div class="d-flex success-checkout align-items-center justify-content-center">
      <div class="col col-lg-4 text-center">
        <img src="img/success-buy.png" alt width="294" />
        <h3 class="mt-4">Payment Successful</h3>
        <p
          class="mt-2"
        >Please check your email for details.</p>
        <router-link to="/" class="primary-btn pd-cart mt-3">Back to Home</router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: "Success"
}
</script>