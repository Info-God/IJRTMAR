<template>
  <div>
    <div class="accordion" role="tablist">
      <b-card no-body class="mb-1">
        <b-card-header header-tag="header" class="p-1" role="tab">
          <b-button block v-b-toggle.accordion-7 variant="info"
            >Open Access license Policy<b-icon-arrow-down></b-icon-arrow-down>
          </b-button>
        </b-card-header>
        <b-collapse
          id="accordion-7"
          visible
          accordion="my-accordion"
          role="tabpanel"
        >
          <b-card-body>
            <b-card-text>
              <div>
                <p>
                  <b
                    >The International Journal of Recent Trends in
                    Multidisciplinary Research (IJRTMR)
                  </b>
                  is loyal to open access to academic work. All the original
                  articles and review papers published in this international
                  journal are free to access immediately from the publication
                  date. We don’t charge any fees for readers to download
                  articles and reviews for their educational use.
                </p>
              </div>
              <div>
                <h5>Benefits of open access for authors, include:</h5>
                <ul>
                  <li><p>Free access for all users worldwide</p></li>
                  <li><p>Authors retain copyright to their work</p></li>
                  <li><p>Increased visibility and readership</p></li>
                  <li><p>Rapid publication</p></li>
                  <li><p>No spatial constraints</p></li>
                </ul>
                <p>
                  The IJRTMR also operates under the Creative Commons License
                  CC-BY. This allows for the reproduction of articles, free of
                  charge, with the appropriate citation information. All authors
                  publishing with the International Journal of Recent Trends in
                  Multidisciplinary Research accept these as the terms of
                  publication.
                </p>
              </div>
            </b-card-text>
          </b-card-body>
        </b-collapse>
      </b-card>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.btn-info {
  background-color: #22bbf0;
}
.card {
  border: none;
}
</style>