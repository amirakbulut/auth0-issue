<template>
  <section class="container-container py-5 my-5 threatments">
    <div class="container my-5">
      <div class="container">
        <div class="row">
          <div class="col-md-12 mb-4">
            <h2>Behandelingen</h2>
            <div class="categories mt-3">
              <h3 class="d-inline-block mr-2 text-primary">Alle</h3>
              <h3 class="d-inline-block mr-2">Volwassenen</h3>
              <h3 class="d-inline-block mr-2">Kinderen</h3>
              <h3 class="d-inline-block mr-2">Gezicht</h3>
            </div>
          </div>
          <div class="col-md-6 threatment-item py-3">
            <div class="card py-3 px-4 bg-white">
              <p>
                <strong>Standaard knipbeurt</strong>
              </p>
              <p class="description my-2">Standaard knipbeurt inclusief contour bijwerken.</p>
              <div class="stats">
                <p class="d-inline-block w-auto mr-2">
                  <i class="las la-stopwatch"></i> 30 min.
                </p>
                <p class="d-inline-block w-auto mr-2 price">
                  <i class="las la-euro-sign"></i> 15,-
                </p>
                <p class="d-inline-block mr-2 mt-1">
                  <i class="las la-info-circle"></i>
                  <a href="#">Meer informatie</a>
                </p>
              </div>
            </div>
          </div>
          <div class="col-md-6 threatment-item py-3">
            <div class="card py-3 px-4 bg-white">
              <p>
                <strong>Volledige knipbeurt</strong>
              </p>
              <p class="description my-2">Uitgebreidde knipbeurt inclusief bijwerken van de baard.</p>
              <div class="stats">
                <p class="d-inline-block w-auto mr-2">
                  <i class="las la-stopwatch"></i> 45 min.
                </p>
                <p class="d-inline-block w-auto mr-2 price">
                  <i class="las la-euro-sign"></i> 20,-
                </p>
                <p class="d-inline-block mr-2 mt-1">
                  <i class="las la-info-circle"></i>
                  <a href="#">Meer informatie</a>
                </p>
              </div>
            </div>
          </div>
          <div class="col-md-6 threatment-item py-3">
            <div class="card py-3 px-4 bg-white">
              <p>
                <strong>Gezichtsmasker &amp; stomen</strong>
              </p>
              <p class="description my-2">Heerlijke masker voor een zachte huid.</p>
              <div class="stats">
                <p class="d-inline-block w-auto mr-2">
                  <i class="las la-stopwatch"></i> 30 min.
                </p>
                <p class="d-inline-block w-auto mr-2 price">
                  <i class="las la-euro-sign"></i> 15,-
                </p>
                <p class="d-inline-block mr-2 mt-1">
                  <i class="las la-info-circle"></i>
                  <a href="#">Meer informatie</a>
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="cart-btn-wrapper">
      <div class="container d-block d-md-none">
        <div class="row">
          <div class="col-md-12">
            <button type="button" class="bg-primary w-100 px-5">
              Afspraak afronden
              <i class="las la-arrow-right ml-2"></i>
            </button>
          </div>
        </div>
      </div>
      <button type="button" class="bg-primary w-100 px-5 d-none d-md-block">
        Afspraak afronden
        <i class="las la-arrow-right ml-2"></i>
      </button>
    </div>
  </section>
</template>