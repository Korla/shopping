<template>
  <quasar-layout>
    <div slot="header" class="toolbar">
      <quasar-toolbar-title :padding="1">
        Shopping!
      </quasar-toolbar-title>
    </div>

    <div class="layout-view">
      <div class="layout-padding">
        <div class="list">
          <div class="item" v-for="item in current">
            <div class="item-content">
              <label>
                <quasar-checkbox v-model="item.checked"></quasar-checkbox>
                <input v-model="item.text"/>
              </label>
            </div>
          </div>
        </div>
      </div>
    </div>
  </quasar-layout>
</template>

<script>
export default {
  data () {
    return {
      master: [],
      current: [
        { text: 'Apples', checked: false },
        { text: 'Oranges', checked: false }
      ]
    }
  },
  methods: {
  }
}
</script>

<style lang="styl">
</style>
