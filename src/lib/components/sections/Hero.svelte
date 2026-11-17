<script lang="ts">
  import { ArrowRight, CalendarCheck, MapPin } from '@lucide/svelte';
  import consultation from '$lib/assets/consultation.webp';
</script>

<section class="hero" aria-labelledby="hero-title">
      <div class="wrap hero-grid">
        <div>
          <p class="eyebrow">Cabinet de nutrition et de diététique</p>
          <h1 id="hero-title">Mieux manger, <span>à votre rythme.</span></h1>
          <p class="hero-lead">Des repères concrets pour une alimentation équilibrée, adaptée à vos habitudes et à votre quotidien.</p>
          <div class="hero-actions">
            <a class="button button-primary" data-appointment href="#contact">
              Prendre rendez-vous
              <ArrowRight class="icon" aria-hidden="true" />
            </a>
            <a class="button button-secondary" href="#prestations">Découvrir les prestations</a>
          </div>
        </div>
        <figure class="hero-photo">
          <img src={consultation} width="1280" height="960" alt="Une diététicienne échange avec une personne autour d’une table, près d’un panier de fruits et légumes." fetchpriority="high">
          <figcaption class="photo-caption">Photo d’illustration</figcaption>
        </figure>
      </div>
      <div class="wrap visit-bar">
        <div class="visit-item">
          <CalendarCheck class="icon icon-large" aria-hidden="true" />
          <div>
            <strong>Consultations sur rendez-vous</strong>
            <p>Le cabinet confirme votre créneau</p>
          </div>
        </div>
        <div class="visit-item">
          <MapPin class="icon icon-large" aria-hidden="true" />
          <strong>Cameroun</strong>
        </div>
        <a class="text-link" href="#contact">
          Informations pratiques
          <ArrowRight class="icon" aria-hidden="true" />
        </a>
      </div>
    </section>
