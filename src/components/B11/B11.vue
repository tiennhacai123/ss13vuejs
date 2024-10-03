<template>
  <div>
    <h2>B11</h2>
    <v-container>
      <v-row>
        <v-col cols="3">
          <v-card>
            <v-card-title>Gender</v-card-title>
            <v-list>
              <v-list-item>All</v-list-item>
              <v-list-item>Kitchen</v-list-item>
              <v-list-item>Electronics</v-list-item>
            </v-list>

            <v-card-title>Colors</v-card-title>
            <v-list>
              <v-list-item>Red</v-list-item>
              <v-list-item>Blue</v-list-item>
              <v-list-item>Black</v-list-item>
            </v-list>

            <v-card-title>Price</v-card-title>
            <v-list>
              <v-list-item>$10 - $50</v-list-item>
              <v-list-item>$50 - $100</v-list-item>
              <v-list-item>$100 - $150</v-list-item>
              <v-list-item>$150 - $200</v-list-item>
              <v-list-item>Over $200</v-list-item>
            </v-list>

            <v-card-title>Rating</v-card-title>
            <v-rating value="4"></v-rating>

            <v-btn color="primary" class="mt-3">Reset Filters</v-btn>
          </v-card>
        </v-col>

        <v-col cols="9">
          <v-card>
            <v-card-title>Products</v-card-title>

            <v-row>
              <v-col cols="4">
                <v-card>
                  <v-img
                    src="https://cutedressy.com/cdn/shop/products/1_e6faeaff-97fb-4cbd-bd01-507b374f4394.jpg"
                    alt="MacBook Air Pro"
                  ></v-img>
                  <v-card-subtitle>MacBook Air Pro</v-card-subtitle>
                  <v-card-text>
                    <div>
                      $15 <span class="text-decoration-line-through">$32</span>
                    </div>
                    <v-rating value="4" small></v-rating>
                  </v-card-text>
                </v-card>
              </v-col>

              <v-col cols="4">
                <v-card>
                  <v-img
                    src="https://cutedressy.com/cdn/shop/products/1_e6faeaff-97fb-4cbd-bd01-507b374f4394.jpg"
                    alt="Red Velvet Dress"
                  ></v-img>
                  <v-card-subtitle>Red Velvet Dress</v-card-subtitle>
                  <v-card-text>
                    <div>
                      $16
                      <span class="text-decoration-line-through">$14.59</span>
                    </div>
                    <v-rating value="5" small></v-rating>
                  </v-card-text>
                </v-card>
              </v-col>

              <v-col cols="4">
                <v-card>
                  <v-img
                    src="https://cutedressy.com/cdn/shop/products/1_e6faeaff-97fb-4cbd-bd01-507b374f4394.jpg"
                    alt="Boat Headphone"
                  ></v-img>
                  <v-card-subtitle>Boat Headphone</v-card-subtitle>
                  <v-card-text>
                    <div>
                      $36 <span class="text-decoration-line-through">$29</span>
                    </div>
                    <v-rating value="5" small></v-rating>
                  </v-card-text>
                </v-card>
              </v-col>

              <v-col cols="4">
                <v-card>
                  <v-img
                    src="https://cutedressy.com/cdn/shop/products/1_e6faeaff-97fb-4cbd-bd01-507b374f4394.jpg"
                    alt="The Psychology of Money"
                  ></v-img>
                  <v-card-subtitle>The Psychology of Money</v-card-subtitle>
                  <v-card-text>
                    <div>
                      $85 <span class="text-decoration-line-through">$49</span>
                    </div>
                    <v-rating value="5" small></v-rating>
                  </v-card-text>
                </v-card>
              </v-col>

              <v-col cols="4">
                <v-card>
                  <v-img
                    src="https://cutedressy.com/cdn/shop/products/1_e6faeaff-97fb-4cbd-bd01-507b374f4394.jpg"
                    alt="Psalms Book for Growth"
                  ></v-img>
                  <v-card-subtitle>Psalms Book for Growth</v-card-subtitle>
                  <v-card-text>
                    <div>$89</div>
                    <v-rating value="5" small></v-rating>
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="4">
                <v-card>
                  <v-img
                    src="https://cutedressy.com/cdn/shop/products/1_e6faeaff-97fb-4cbd-bd01-507b374f4394.jpg"
                    alt="Gaming Console"
                  ></v-img>
                  <v-card-subtitle>Gaming Console</v-card-subtitle>
                  <v-card-text>
                    <div>
                      $99 <span class="text-decoration-line-through">$86</span>
                    </div>
                    <v-rating value="4" small></v-rating>
                  </v-card-text>
                </v-card>
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script setup></script>

<style scoped>
.v-card-subtitle {
  font-weight: bold;
}

.v-card-text {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.text-decoration-line-through {
  text-decoration: line-through;
}
</style>
