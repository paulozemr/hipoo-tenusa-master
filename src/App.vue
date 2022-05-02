<script>
import CalculosHipotenusa from "@/components/CalculosHipotenusa.vue";
import CAbeça from "@/components/CAbeça.vue";
import FootTwister from "@/components/FootTwister.vue";
import ContenteTv from "@/components/ContenteTv.vue";
export default {
  components: { CalculosHipotenusa, CAbeça, FootTwister, ContenteTv },
};
</script>
<template>
  <CAbeça />
  <CalculosHipotenusa />
  <ContenteTv />
  <FootTwister></FootTwister>
</template>
