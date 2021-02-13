<template>
  <div class="zones-intervencio">
    <div class="zones-intervencio__item">
      <img src="~static/img/zonauno.png" />
      <div class="zones-intervencio__text" style="text-align: right;">
        <h3>ZONES D'INTERVENCIÓ</h3>
        <p>
          Una primera zona d’intervenció que redundaria en un benefici general
          per al Delta seria la conca de l’Ebre. La zona d’intervenció
          inicialment es limitaria a l’aprofitament dels sediments acumulats als
          embassaments de Riba-Roja i Mequinensa, si bé es necessària una
          política correcta de gestió sostenible dels sediments en tots els
          embassaments de la conca.
        </p>
      </div>
    </div>
    <div class="zones-intervencio__item">
      <div class="zones-intervencio__text">
        <p>
          En el cas de les intervencions al delta de l’Ebre, el criteris
          empleats són: processos litorals dominants (zones d'erosió envers
          l'acreció litoral), Capacitat dinàmica i de resposta dels sistemes
          naturals (interior de les badies envers el front litoral), Impactes
          dels fenòmens erosius i d'inundació costanera (ambientals, econòmics,
          etc.).
        </p>
        <p>
          D’aquesta manera s’han identificat 15 sectors diferents a la costa del
          Delta:
        </p>
      </div>

      <img src="~static/img/zonados.png" />
    </div>
  </div>
</template>

<script>
export default {};
</script>
<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

.zones-intervencio {
  background-color: variables.$background-green;
  padding: 3rem 0rem;
  width: 100%;

  &__item {
    background-color: variables.$background-green-dark;
    display: flex;
    width: 100%;
    margin: 2rem 0rem;
  }

  &__text{
    padding: 3rem;
  }
}
</style>