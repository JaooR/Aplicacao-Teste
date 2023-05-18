<template>
  <q-page class="text-center text-italic">
    <div class="flex flex-center" style="font-size: 25px;">
      <div style="background-color: #1976D2; border-radius: 20px; width: 238px; margin-top: 15px;">
        <div style="color: white; font-size: 18px; margin-bottom: 18px; margin-top: 19px;">
          Histórico
        </div>
      </div>
    </div>
    <div style="margin-top: 25px;">
      <q-table class="flex" title="" :rows="rows" :columns="columns" row-key="name" />
    </div>
  </q-page>
</template>

<script setup>
const columns = [
  { name: 'codigo', field: 'codigo', label: 'Codigo' },
  { name: 'identificacao', field: 'identificacao', label: 'Identificação' },
  { name: 'inquilino', field: 'inquilino', label: 'Inquilino' },
  { name: 'data_de_retirada', field: 'data_de_retirada', label: 'Data de Retirada' },
];
const rows = [
  {
    codigo: '1',
    identificacao: 'Kabum',
    inquilino: 'Pedro',
    data_de_retirada: '23/03/2023',
  },
  {
    codigo: '2',
    identificacao: 'Mercado Livre',
    inquilino: 'Pedro',
    data_de_retirada: '23/03/2023',
  },
];
</script>
