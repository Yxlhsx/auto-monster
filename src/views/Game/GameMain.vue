<script lang="ts" setup>
import StatsPanel from "./Panel/StatsPanel.vue";
import EquipmentPanel from "./Panel/EquipmentPanel.vue";
import BagPanel from "./Panel/BagPanel.vue";
import FightLogPanel from "./Panel/FightLogPanel.vue";

const { t } = useI18n();
</script>

<template>
  <div h-full w-screen color-white p2 flex gap-2>
    <div hw-full flex flex-col border-solid-base gap-2 p2>
      <div w-full flex gap-2 flex-1>
        <StatsPanel />
        <EquipmentPanel />
      </div>
      <div w-full flex-1>
        <BagPanel />
      </div>
    </div>
    <div hw-full flex border-solid-base>
      <FightLogPanel />
    </div>
  </div>
</template>
