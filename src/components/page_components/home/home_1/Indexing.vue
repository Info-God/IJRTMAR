<template>
  <div>
    <div class="col-12 p-4 ImageContainer">
      <div class="col-12 row mx-auto justify-center" style="justify-content: center;">
        <div class="col-lg-2 col-md-3 col-sm-3  indexingImage single-pricing-table" v-for="data in indexingList"
          :key="data.indexing_id" v-b-tooltip.hover.bottom @click="openIndexingURL(data.indexing_url)"
          :title="data.indexing_name">
          <img alt="image" :src="data.indexing_image_url" class="rounded mx-auto d-block" width="350" height="250" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Blogs",
  components: {
  },
  data: function () {
    return {
      indexingList: [],
    };
  },
  methods: {
    openIndexingURL: function (indexingURL) {
      window.open(indexingURL, "_blank");
    },
    getIndexing: function () {
      this.api.postData("indexfetch").then((res) => {
        this.indexingList = res.data.indexingList;
      },
        (err) => {
          console.log(err);
        }
      );
    },
  },
  mounted: function () {
    this.getIndexing();
  },
};
</script>

<style scoped>
.ImageContainer {
  padding-left: 50px !important;
}

.indexingImage {
  margin: 10px;
  transition: 0.5s;
  cursor: pointer;
}

.indexingImage img {
  padding: 10px;
  height: 100%;
  width: 100%;
  box-shadow: rgba(0, 0, 0, 0.3) 0px 5px 25px,
    rgba(0, 0, 0, 0.22) 0px 15px 12px;
}

.single-pricing-table:hover {
  transform: translateY(-10px);
  box-shadow: none;
}
</style>