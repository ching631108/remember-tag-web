<template>
    <div class="w-full h-32 bg-white flex flex-col justify-between border-b-2 border-gray-100 mb-2 pb-1 hover:bg-gray-200 p-2 cursor-pointer">
        <!-- 标题 -->
      <div class="flex justify-between mb-0.5">
        <div class="text-xl font-medium text-black">{{ title }}</div>
        <div class="text-sm text-gray-400">{{ showTime }}</div>
      </div>
      <div class="justify-start">
        <div class="text-base text-gray-800 text-left px-2">{{ description }}</div>
      </div>
      <div class="flex justify-end">
        <div class="text-sm text-gray-800">总数：{{ total }}</div>
        <div class="text-sm text-gray-800 ml-2">已完成：{{ finish }}</div>
      </div>
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
  ]
}
</script>
