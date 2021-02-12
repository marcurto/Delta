<template>
  <div class="noticies">
    <News />
    <News date="1-12-2019" title="La Taula del Delta demana 6 milions contra la regressió" subtitle="Els alcaldes d’Amposta, Deltebre i Sant Jaume i els presidents de les comunitats de regants es reuneixen amb la ministra Teresa Ribera" href="https://www.diaridetarragona.com/ebre/La-Taula-del-Delta-demana-6-milions-contra-la-regressio-20191219-0032.html"/>
    <News date="19-12-2019" title="La Taula de Consens demana al Ministeri 6 milions d'euros per a accions urgents contra la regressió al Delta" subtitle="Una representació de la Taula va reunir-se dimecres a Madrid amb la ministra de Transició Ecològica Teresa Ribera" href="https://www.setmanarilebre.cat/noticia/110215/la-taula-de-consens-demana-al-ministeri-6-milions-deuros-per-a-accions-urgents-contra-la-r"/>
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
