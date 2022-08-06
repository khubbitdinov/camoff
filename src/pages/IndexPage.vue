<template>
  <q-page>
    <div class="row ">
      <div v-for="item in camList" :key="item" class="col-6 q-pa-sm">
        <q-card class="my-card">
          <q-card-section class="cardColor text-white">
            <div class="text-h6">{{item.number}}</div>
            <div class="text-subtitle2">{{item.name}}</div>
          </q-card-section>

          <q-card-actions align="around">
            <q-btn flat>Выкл</q-btn>
            <q-btn flat>Вкл</q-btn>
          </q-card-actions>
        </q-card>
      </div>
    </div>

  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  data: () => ({
    camList: [
      {
        id: `00000001-0000-0000-0000-000000000000`,
        name: `Вход`,
        number: 1,
      },
      {
        id: `00000002-0000-0000-0000-000000000000`,
        name: `Задний двор хоз блок`,
        number: 2,
      },
      {
        id: `00000003-0000-0000-0000-000000000000`,
        name: `Задний двор мусорка`,
        number: 3,
      },
      {
        id: `00000004-0000-0000-0000-000000000000`,
        name: `Задний двор ворота`,
        number: 4,
      },
      {
        id: `00000005-0000-0000-0000-000000000000`,
        name: `2эт изм обвод`,
        number: 5,
      },
      {
        id: `00000006-0000-0000-0000-000000000000`,
        name: `2эт администрация`,
        number: 6,
      },
      {
        id: `00000007-0000-0000-0000-000000000000`,
        name: `2эт коридор`,
        number: 7,
      },
      {
        id: `00000008-0000-0000-0000-000000000000`,
        name: `2эт изм отобвод`,
        number: 8,
      },
      {
        id: `00000009-0000-0000-0000-000000000000`,
        name: `3эт коридор`,
        number: 9,
      },
      {
        id: `0000000A-0000-0000-0000-000000000000`,
        name: `5эт коридор`,
        number: 10,
      },
      {
        id: `0000000B-0000-0000-0000-000000000000`,
        name: `4эт изм отобвод`,
        number: 11,
      },
      {
        id: `0000000C-0000-0000-0000-000000000000`,
        name: `4эт изм обвод`,
        number: 12,
      },
      {
        id: `0000000D-0000-0000-0000-000000000000`,
        name: `6эт коридор`,
        number: 13,
      },
      {
        id: `0000000E-0000-0000-0000-000000000000`,
        name: `6э изм отобвод`,
        number: 14,
      },
      {
        id: `0000000F-0000-0000-0000-000000000000`,
        name: `4эт коридор`,
        number: 15,
      },
      {
        id: `00000010-0000-0000-0000-000000000000`,
        name: `6эт изм обвод`,
        number: 16,
      }
    ]
  })
})
</script>
