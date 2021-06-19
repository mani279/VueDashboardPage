<template>
  <q-item :active="active" active-class="bg-primary"
    
  >
    <q-item-section
      v-if="icon"
      avatar
    >
      <q-icon class="text-white" :name="icon" />
    </q-item-section>

    <q-item-section>
      <q-item-label class="text-white">{{ title }}</q-item-label>
    </q-item-section>
  </q-item>
</template>

<script>
export default {
  name: 'EssentialLink',
  props: {
    active:{
      type: Boolean,
      default:true 
    },
    title: {
      type: String,
      required: true
    },

    caption: {
      type: String,
      default: ''
    },

    link: {
      type: String,
      default: '#'
    },

    icon: {
      type: String,
      default: ''
    },
  }
}
</script>
