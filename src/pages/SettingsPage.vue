<template>
  <q-page class="window-height window-width row justify-center items-center">
    <div class="q-pa-sm window-width" >
      <q-form class="q-py-sm">
        <q-input square filled clearable v-model="form.ip" type="ip" label="ip" />
        <q-input square filled clearable v-model="form.email" type="login" label="login" />
        <q-input square filled clearable v-model="form.password" type="password" label="password" />
      </q-form>
      <q-btn outline class="full-width" @click="save" label="Сохранить"/>
    </div>
  </q-page>
</template>

<script>
export default {
  name: "SettingsPage",
  data: () => ({
    form: {
      ip: '',
      email: '',
      password: '',
    },
  }),
  methods: {
    save() {
      this.$q.localStorage.set('settings',this.form)
    }
  },
  mounted() {
    this.form = this.$q.localStorage.getItem('settings')
  }
};
</script>

<style scoped>

</style>
