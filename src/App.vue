<template>
  <div id="app">
    <product-details :product="product" />
    <product-tabs-info
      :content="product.content"
      :productInfo="product.product_info"
      :review="product.review"
    />
  </div>
</template>

<script>
import ProductDetails from "./components/ProductDetails.vue";
import ProductTabsInfo from "./components/ProductTabsInfo.vue";

export default {
  name: "App",
  data() {
    return {
      product: {
        id: 1,
        title: "Samsung Galaxy Note 10",
        description: "Provided by Samsung, Ltd",
        rating: 4,
        variants: [
          {
            image:
              "https://galaxydidong.vn/wp-content/uploads/2020/04/samsung-galaxy-z-flip-den-600x600-600x600.jpg",
            price: 20,
            id: 1,
            quatity: 4,
          },
          {
            image:
              "https://toanmobile.vn/userdata/8264/wp-content/uploads/2021/10/samsung-galaxy-s8-plus-hh-600x600-600x600.jpg",
            price: 30,
            id: 2,
            quatity: 2,
          },
        ],
        content: ` The Corsair Gaming Series GS600 power supply is the ideal
            price-performance solution for building or upgrading a Gaming PC. A
            single +12V rail provides up to 48A of reliable, continuous power
            for multi-core gaming PCs with multiple graphics cards. The
            ultra-quiet, dual ball-bearing fan automatically adjusts its speed
            according to temperature, so it will never intrude on your music and
            games. Blue LEDs bathe the transparent fan blades in a cool glow.
            Not feeling blue? You can turn off the lighting with the press of a
            button.

            <h3>Corsair Gaming Series GS600 Features:</h3>
            <li>
              It supports the latest ATX12V v2.3 standard and is backward
              compatible with ATX12V 2.2 and ATX12V 2.01 systems
            </li>
            <li>
              An ultra-quiet 140mm double ball-bearing fan delivers great
              airflow at an very low noise level by varying fan speed in
              response to temperature
            </li>
            <li>
              80Plus certified to deliver 80% efficiency or higher at normal
              load conditions (20% to 100% load)
            </li>
            <li>
              0.99 Active Power Factor Correction provides clean and reliable
              power
            </li>
            <li>
              Universal AC input from 90~264V — no more hassle of flipping that
              tiny red switch to select the voltage input!
            </li>
            <li>Extra long fully-sleeved cables support full tower chassis</li>
            <li>
              A three year warranty and lifetime access to Corsair’s legendary
              technical support and customer service
            </li>
            <li>
              Over Current/Voltage/Power Protection, Under Voltage Protection
              and Short Circuit Protection provide complete component safety
            </li>
            <li>Dimensions: 150mm(W) x 86mm(H) x 160mm(L)</li>
            <li>MTBF: 100,000 hours</li>
            <li>
              Safety Approvals: UL, CUL, CE, CB, FCC Class B, TÜV, CCC, C-tick
            </li>`,
        product_info:
          "[Product info] In publishing and graphic design, Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content. Lorem ipsum may be used as a placeholder before final copy is available. Wikipedia",
        review:
          "[Review] In publishing and graphic design, Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document or a typeface without relying on meaningful content. Lorem ipsum may be used as a placeholder before final copy is available. Wikipedia",
      },
    };
  },
  components: {
    ProductDetails,
    ProductTabsInfo,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
