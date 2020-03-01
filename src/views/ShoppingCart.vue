<template>
  <div>
    <HeaderLunaShop />
    <!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-left">
            <div class="breadcrumb-text product-more">
              <router-link to="/">
                <i class="fa fa-home"></i> Home
              </router-link>
              <span>Shopping Cart</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Shopping Cart Section Begin -->
    <section class="shopping-cart spad">
      <div class="container">
        <div class="row">
          <div class="col-lg-8">
            <div class="row">
              <div class="col-lg-12">
                <div class="cart-table">
                  <table>
                    <thead>
                      <tr>
                        <th>Image</th>
                        <th class="p-name text-center">Product Name</th>
                        <th>Price</th>
                        <th>Action</th>
                      </tr>
                    </thead>
                    <tbody>
                      <tr>
                        <td class="cart-pic first-row">
                          <img src="images/products/samsung-galaxy-note-10-plus-thumb.jpg" />
                        </td>
                        <td class="cart-title first-row text-center">
                          <h5>Samsung Galaxy Note10+ 256GB - Aura Black</h5>
                        </td>
                        <td class="p-price first-row">Rp 16.099.000</td>
                        <td class="delete-item">
                          <a href="#">
                            <i class="material-icons">close</i>
                          </a>
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </div>
              </div>
              <div class="col-lg-8">
                <h4 class="mb-4 text-left">Buyer Information:</h4>
                <div class="user-checkout text-left">
                  <form>
                    <div class="form-group">
                      <label for="fullName">Full Name</label>
                      <input
                        type="text"
                        class="form-control"
                        id="fullName"
                        aria-describedby="nameHelp"
                        placeholder="Input your name..."
                      />
                    </div>
                    <div class="form-group">
                      <label for="emailAddress">Email Address</label>
                      <input
                        type="email"
                        class="form-control"
                        id="emailAddress"
                        aria-describedby="emailHelp"
                        placeholder="Input your email..."
                      />
                    </div>
                    <div class="form-group">
                      <label for="phoneNumber">Phone Number</label>
                      <input
                        type="text"
                        class="form-control"
                        id="phoneNumber"
                        aria-describedby="phoneNumberHelp"
                        placeholder="Input your phone number..."
                      />
                    </div>
                    <div class="form-group">
                      <label for="address">Address</label>
                      <textarea class="form-control" id="address" rows="3"></textarea>
                    </div>
                  </form>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-4">
            <div class="row">
              <div class="col-lg-12">
                <div class="proceed-checkout text-left">
                  <ul>
                    <li class="subtotal">
                      Transaction ID
                      <span>#LUNA000000001</span>
                    </li>
                    <li class="subtotal mt-3">
                      Subtotal
                      <span>Rp 16.099.000</span>
                    </li>
                    <li class="subtotal mt-3">
                      Tax
                      <span>10%</span>
                    </li>
                    <li class="subtotal mt-3">
                      Grand Total
                      <span>Rp 17.708.900</span>
                    </li>
                    <li class="subtotal mt-3">
                      Bank Transfer
                      <span>BCA</span>
                    </li>
                    <li class="subtotal mt-3">
                      Bank Account
                      <span>8830 792 920</span>
                    </li>
                    <li class="subtotal mt-3">
                      Seller Name
                      <span>LunaShop</span>
                    </li>
                  </ul>
                  <router-link to="/success" class="proceed-btn">I ALREADY PAID</router-link>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Shopping Cart Section End -->
    <FooterLunaShop />
  </div>
</template>

<script>
import HeaderLunaShop from "@/components/HeaderLunaShop.vue";
import FooterLunaShop from "@/components/FooterLunaShop.vue";

export default {
  name: "ShoppingCart",
  components: {
    HeaderLunaShop,
    FooterLunaShop
  }
};
</script>