<template>
  <div class="container">
    <Manufacturer v-slot="data">
      <Devices :manufacturerId="data.factId"></Devices>
    </Manufacturer>
  </div>
</template>

<script>
import Manufacturer from "@/components/Manufacuturer.vue";
import Devices from "@/components/Devices.vue";
export default {
  components: {
    //name: file,
    Manufacturer: Manufacturer,
    Devices: Devices,
  },
};
</script>