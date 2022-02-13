<template>
 <div class="w-72 bg-white rounded shadow-2xl">
    <!-- image -->
    <div class="h-48 bg-gray-200 rounded-tr rounded-tl">
        <img src="~@/assets/images/tanjiro.jpg" class="h-48 w-full object-fill" alt="Tanjiro Kamado">
    </div>

    <div class="p-5">
      <!-- title -->
      <div class="h-6 rounded-sm mb-4">
        <h1 class="font-semibold text-gray-600 text-lg">Tanjiro Kamado</h1>
      </div>

      <!-- content -->
      <div class="text-left">
        <div class="h-42 bg-gray-200 rounded-sm px-2">
          <p class="break-words">A jornada de Tanjiro tem como fio principal 2 objetivos:</p>
          <p>transformar sua irmã novamente em humana e se vingar do demônio que destruiu sua família.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang='ts'>
import { defineComponent } from 'vue';

const Card = defineComponent({
});

export default Card;
</script>

<style>

</style>