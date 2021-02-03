<template>
    <div class="relative">
      <CardListItem
        v-for="(oneItem, index) of listData"
        :key="index"
        :title="oneItem.title"
        :description="oneItem.description"
        :showTime="oneItem.showTime"
        :total="oneItem.total"
        :finish="oneItem.finish"
      />
      <AddButton
        class="fixed bottom-5 right-1/2 -mr-44"
      >
        <div class="py-2 hover:bg-blue-700" @click="addGroupBtnHandler">新增标签组</div>
        <div class="py-2 hover:bg-blue-700" @click="addTagBtnHandler">新增标签</div>
      </AddButton>
    </div>
</template>

<script>
import AddButton from '@/components/CardList/AddButton'
import CardListItem from '@/components/CardList/CardListItem'
export default {
  name: 'Home',
  components: {
    CardListItem,
    AddButton
  },
  data: () => {
    return {
      listData: [{
        title: '五十音卡片组', // 标题
        description: '其中包含日语基本的平假名和片假名中的内容，包含清音和浊音', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语四级速成词汇', // 标题
        description: '其中包含英语四级的基础词汇', // 描述
        showTime: '2020-05-21', // 展示时间
        total: '130', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语雅思速成词汇', // 标题
        description: '其中包含雅思的高级语法和词汇', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }, {
        title: '五十音卡片组', // 标题
        description: '其中包含日语基本的平假名和片假名中的内容，包含清音和浊音', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语四级速成词汇', // 标题
        description: '其中包含英语四级的基础词汇', // 描述
        showTime: '2020-05-21', // 展示时间
        total: '130', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语雅思速成词汇', // 标题
        description: '其中包含雅思的高级语法和词汇', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }, {
        title: '五十音卡片组', // 标题
        description: '其中包含日语基本的平假名和片假名中的内容，包含清音和浊音', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语四级速成词汇', // 标题
        description: '其中包含英语四级的基础词汇', // 描述
        showTime: '2020-05-21', // 展示时间
        total: '130', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语雅思速成词汇', // 标题
        description: '其中包含雅思的高级语法和词汇', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }, {
        title: '五十音卡片组', // 标题
        description: '其中包含日语基本的平假名和片假名中的内容，包含清音和浊音', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语四级速成词汇', // 标题
        description: '其中包含英语四级的基础词汇', // 描述
        showTime: '2020-05-21', // 展示时间
        total: '130', // 总数
        finish: '15' // 已完成
      }, {
        title: '英语雅思速成词汇', // 标题
        description: '其中包含雅思的高级语法和词汇', // 描述
        showTime: '2021-05-21', // 展示时间
        total: '68', // 总数
        finish: '15' // 已完成
      }]
    }
  },
  methods: {
    addGroupBtnHandler: () => {
      // @todo 完成点击新增分组按钮逻辑
    },
    addTagBtnHandler: () => {
      // @todo 完成点击新增标签按钮逻辑
    }
  }
}
</script>
