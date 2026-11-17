<script lang="ts">
  import { ClipboardList, Sprout } from '@lucide/svelte';
</script>

<section class="services" id="prestations" aria-labelledby="services-title" tabindex="-1">
      <div class="wrap">
        <div class="section-heading">
          <h2 id="services-title">Nos prestations</h2>
          <p>Prestations à confirmer auprès du cabinet.</p>
        </div>
        <div class="services-grid">
          <article class="service-card">
            <div class="service-icon">
              <ClipboardList class="icon icon-large" aria-hidden="true" />
            </div>
            <div>
              <h3>Consultation initiale</h3>
              <p>Faire le point sur vos habitudes alimentaires et définir avec vous les premières étapes.</p>
            </div>
          </article>
          <article class="service-card">
            <div class="service-icon service-icon-warm">
              <Sprout class="icon icon-large" aria-hidden="true" />
            </div>
            <div>
              <h3>Suivi diététique</h3>
              <p>Ajuster vos repères au fil du temps selon vos progrès, vos questions et vos contraintes.</p>
            </div>
          </article>
        </div>
      </div>
    </section>
