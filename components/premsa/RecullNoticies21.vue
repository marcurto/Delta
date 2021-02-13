<template>
  <div class="noticies">
    <News date="11-01-2021" title="La disputa entre la Generalitat i el Ministeri bloqueja el pla de xoc per salvar el delta de l’Ebre" subtitle="El Govern es queixa que no rep el permís per actuar mentre que Transició Ecològica demana concreció en el projecte" href="https://cat.elpais.com/cat/2021/01/11/catalunya/1610381939_134848.html"/>
    <News date="11-01-2021" title="Alcaldes del delta del Ebro denuncian “inacción” ante los nuevos daños por ‘Filomena’" subtitle="El temporal ha afectado a las zonas más vulnerables" href="El Govern es queixa que no rep el permís per actuar mentre que Transició Ecològica demana concreció en el projecte"/>
    <News date="21-01-2021" title="El Delta pide auxilio y carga contra la inacción pública" subtitle="Los siete municipios del humedal ebrense y los regantes critican a Govern y Ministerio por dejar que el mar se coma la franja costera" href="https://www.lavanguardia.com/local/tarragona/20210121/6186276/delta-auxilio-inaccion-politica-gloria-filomena.html"/>
    <News date="22-01-2021" title="La Taula de Consens obre la porta a iniciar la defensa legal per salvar el Delta de l'Ebre" subtitle="Els ajuntaments deltaics i les comunitats de regants realitzen un ple simultani per aprovar també futures mobilitzacions" href="https://www.google.com/url?q=https://www.aguaita.cat/noticia/20523/taula-consens-obre-porta-iniciar-defensa-legal-salvar-delta-ebre&sa=D&source=editors&ust=1613145082096000&usg=AOvVaw2DLQp0FDNbTBPXN41-6_8F"/>
    <News date="23-01-2021" title="La Taula de Consens pel Delta es reuneix amb les ja més de 30 entitats adherides" subtitle="De la reunió es va reafirmar la unió que mostra el territori i el suport als plantejaments a la Taula de Consens." href="https://www.google.com/url?q=https://www.imaginaradio.cat/la-taula-de-consens-pel-delta-es-reuneix-amb-les-ja-mes-de-30-entitats-adherides/&sa=D&source=editors&ust=1613145098653000&usg=AOvVaw3ftRcsTJI7axJxmd_5MS0_"/>
    <News date="29-01-2021" title="Entrevista a Rafa Sánchez, director tècnic i portaveu de la Taula de Consens  " subtitle="El Delta preocupa i molt, sobretot des que el temporal Gloria primer i el Filomena després, van posar sota el focus mediàtic els problemes endèmics que arrossega des de fa molts anys" href="https://deltacat.cat/2021/01/29/entrevista-a-rafa-sanchez-director-tecnic-i-portaveu-de-la-taula-de-consens-29-01-2021/"/>

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
