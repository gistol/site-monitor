<template>
  <div :class="componentClass">
    <span class="siteList__single__title">Actions</span>
    <a :href="`site/${site.id}`">
      <i class="ion-md-create"></i>
      <span>Edit</span>
    </a>
  </div>
</template>

<script>
  export default {
    name: 'Actions',

    props: [
      'cssClass',
      'site'
    ],

    computed: {
      componentClass() {
        return this.cssClass ? this.cssClass + '__actions' : 'actions';
      }
    },
  }
</script>