<template>
    <div class="transition-all text-white bg-blue-500"
        :class="classObject"
         @click="clickHandler"
    >
       <div v-if="!showMenu" class="flex justify-center items-center h-10">
            <span class="text-lg">+</span>
       </div>
       <slot v-if="showMenu"></slot>
    </div>
</template>

<script>

export default {
  props: [
    'title', // 标题
    'description', // 描述
    'showTime', // 展示时间
    'total', // 总数
    'finish' // 已完成
  ],
  data: () => {
    return {
      showMenu: false,
      classObject: {
        rounded: false,
        'w-32': false,
        'max-h-96': false,

        'w-10': true,
        'max-h-10': true,
        'rounded-full': true
      }
    }
  },
  methods: {
    clickHandler () {
      this.showMenu = true
    }
  },
  watch: {
    showMenu (newVal) {
      this.classObject.rounded = newVal
      this.classObject['w-32'] = newVal
      this.classObject['max-h-96'] = newVal

      this.classObject['w-10'] = !newVal
      this.classObject['max-h-10'] = !newVal
      this.classObject['rounded-full'] = !newVal
    }
  }
}
</script>
