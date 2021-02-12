<template>
  <div class="noticies">
    <News date="11-01-2021" title="La disputa entre la Generalitat i el Ministeri bloqueja el pla de xoc per salvar el delta de l’Ebre" subtitle="El temporal ha afectado a las zonas más vulnerables"/>
    <News date="11-01-2021" title="Alcaldes del delta del Ebro denuncian “inacción” ante los nuevos daños por ‘Filomena’" subtitle="Los siete municipios del humedal ebrense y los regantes critican a Govern y Ministerio por dejar que el mar se coma la franja costera"/>
    <News date="21-01-2021" title="El Delta pide auxilio y carga contra la inacción pública" subtitle="Els ajuntaments deltaics i les comunitats de regants realitzen un ple simultani per aprovar també futures mobilitzacions"/>
    <News date="22-01-2021" title="La Taula de Consens obre la porta a iniciar la defensa legal per salvar el Delta de l'Ebre" subtitle="El Delta preocupa i molt, sobretot des que el temporal Gloria primer i el Filomena després, van posar sota el focus mediàtic els problemes endèmics que arrossega des de fa molts anys"/>
    <News date="23-01-2021" title="La Taula de Consens pel Delta es reuneix amb les ja més de 30 entitats adherides" subtitle="El Delta preocupa i molt, sobretot des que el temporal Gloria primer i el Filomena després, van posar sota el focus mediàtic els problemes endèmics que arrossega des de fa molts anys"/>
    <News date="29-01-2021" title="Entrevista a Rafa Sánchez, director tècnic i portaveu de la Taula de Consens  " subtitle="El Delta preocupa i molt, sobretot des que el temporal Gloria primer i el Filomena després, van posar sota el focus mediàtic els problemes endèmics que arrossega des de fa molts anys"/>

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
