<script lang="ts">
  import { CalendarCheck } from '@lucide/svelte';
  import logo from '$lib/assets/logo.webp';
</script>

<header class="site-header">
    <div class="wrap masthead">
      <a class="brand" href="#accueil" aria-label="Délice Diet, accueil">
        <img src={logo} width="42" height="42" alt="">
        <span class="brand-name">Délice <span>Diet</span></span>
      </a>
      <nav class="navigation" id="navigation" aria-label="Navigation principale">
        <ul>
          <li><a href="#accueil">Accueil</a></li>
          <li><a href="#prestations">Prestations</a></li>
          <li><a href="#cabinet">Le cabinet</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
        <a class="button button-primary header-appointment" data-appointment href="#contact">
          <CalendarCheck class="icon" aria-hidden="true" />
          Prendre rendez-vous
        </a>
      </nav>
    </div>
  </header>
