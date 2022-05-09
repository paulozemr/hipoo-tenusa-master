<script>
import CalculosHipotenusa from "@/components/CalculosHipotenusa.vue";
import CAbeca from "@/components/CAbeca.vue";
import FootTwister from "@/components/FootTwister.vue";
import ContenteTv from "@/components/ContenteTv.vue";
export default {
  components: { CalculosHipotenusa, CAbeca, FootTwister, ContenteTv },
};
</script>
<template>
  <CAbeca />
  <CalculosHipotenusa />
  <ContenteTv />
  <FootTwister></FootTwister>
</template>
