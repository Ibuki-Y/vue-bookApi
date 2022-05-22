import GlobalHeader from '@/global/GlobalHeader.vue';
<template>
  <div>
    <v-app-bar app color="primary" dark>
      <v-spacer></v-spacer>
      <v-btn color="error" @click="deleteAll">削除</v-btn>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name:'GlobalHeader',
  methods:{
    deleteAll(){
      this.$emit('delete-all')
    }
  }
};
</script>

<style></style>
