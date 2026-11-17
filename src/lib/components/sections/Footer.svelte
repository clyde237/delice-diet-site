<script lang="ts">
  import { ArrowUp } from '@lucide/svelte';
</script>

<footer class="site-footer">
    <div class="wrap footer-inner">
      <a class="brand" href="#accueil" aria-label="Délice Diet, accueil">
        <span class="brand-name">Délice <span>Diet</span></span>
      </a>
      <p>Cabinet de nutrition et de diététique · Cameroun</p>
    </div>
  </footer>

<a class="back-to-top" href="#accueil" aria-label="Retour en haut de page" title="Retour en haut de page">
  <ArrowUp class="icon" aria-hidden="true" />
</a>

<style>
  .back-to-top {
    position: fixed;
    right: max(1rem, env(safe-area-inset-right));
    bottom: max(1rem, env(safe-area-inset-bottom));
    z-index: 4;
    display: grid;
    width: 3rem;
    height: 3rem;
    place-items: center;
    border: 1px solid rgba(255, 255, 255, 0.4);
    border-radius: 50%;
    background: var(--forest);
    color: white;
    box-shadow: 0 0.4rem 1rem rgba(16, 51, 30, 0.2);
    transition: background-color 160ms ease;
  }

  .back-to-top:hover {
    background: var(--deep-green);
  }

  @media (prefers-reduced-motion: reduce) {
    .back-to-top {
      transition: none;
    }
  }
</style>
