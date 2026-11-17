<script lang="ts">
  import { ArrowRight } from '@lucide/svelte';
  import alimentation from '$lib/assets/alimentation.webp';
</script>

<section class="about" id="cabinet" aria-labelledby="about-title" tabindex="-1">
      <div class="wrap about-grid">
        <img class="about-photo" src={alimentation} width="1056" height="792" alt="Une assiette de riz, haricots, plantain doré et légumes verts." loading="lazy" decoding="async">
        <div class="about-copy">
          <p class="eyebrow">Le cabinet Délice Diet</p>
          <h2 id="about-title">Vos habitudes, notre point de départ.</h2>
          <p>Délice Diet est un cabinet de nutrition et de diététique au Cameroun. L’accompagnement part de vos repas, de vos préférences et des aliments que vous trouvez près de chez vous.</p>
          <a class="text-link" href="#contact">
            Contacter le cabinet
            <ArrowRight class="icon" aria-hidden="true" />
          </a>
        </div>
      </div>
    </section>
