<template>
  <div class="noticies">
    <News date="14-02-2018" title="La NASA alerta de la regressió del delta de l'Ebre" subtitle="L’organisme nord-americà ha publicat un article en què explica els factors que fan perillar el futur de l'indret" href="https://www.naciodigital.cat/noticia/150482/nasa-alerta-regressio-delta-ebre"/>
    <News date="17-07-2018" title="Els regants i alcaldes del delta de l'Ebre reclament un pla de protecció del litoral contra la regressió" subtitle="El document assenyala que 'correspon, de manera urgent i persistent, a les entitats del territori la justa demanda a les administracions pertinents'" href="https://www.ccma.cat/324/els-regants-i-els-alcaldes-del-delta-de-lebre-reclamen-un-pla-de-proteccio-del-litoral-contra-la-regressio/noticia/2867113/"/>
    <News date="18-07-2021" title="Regants i alcaldes del Delta reclament un pla urgent de protecció del litoral" subtitle="Han activat un front comú davant les administracions superiors per lluitar contra la regressió i garantir el futur de la zona" href="https://www.diaridetarragona.com/ebre/Regants-i-alcaldes-del-Delta-reclamen-un-pla-urgent-de-proteccio-del-litoral-20180718-0014.html"/>
    <News date="13-11-2021" title="Acord de mínims entre administracions i regants del delta de l'Ebre per consensuar mesures contra la regressió" subtitle="La constitució formal de l'anomenada Taula de Consens i Territori ha servit per constatar la voluntat d'ajuntaments, Generalitat, govern espanyol i regants de posar sobre la taula solucions efectives" href="https://www.ccma.cat/324/acord-de-minims-entre-administracions-i-regants-del-delta-de-lebre-per-consensuar-mesures-contra-la-regressio/noticia/2886670/"/>
    <News date="14-11-2021" title="La taula contra la regressió del Delta actuarà amb mesures específiques per a cada espai" subtitle="Les dues comunitats de regants i els set municipis deltaics formen aquest ens que busca solucions consensuades contra la regressió del Delta. Es va constituir formalment ahir" href="https://www.diaridetarragona.com/ebre/La-taula-contra-la-regressio-del-Delta-actuar-amb-mesures-especifiques-per-a-cada-espai--20181114-0027.html"/>
  </div>
</template>

<script>
import News from "@/components/ui/molecules/News.vue";

export default {
  components: {
    News,
  },
};
</script>

<style lang="scss" scoped>
@use "@/assets/style/settings/_variables.scss";
@use "@/assets/style/tools/_mixins.scss";
@use "@/assets/style/index.scss";

@import url("https://use.fontawesome.com/releases/v5.9.0/css/all.css");

.news {

}
</style>
