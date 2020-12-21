<template>
   <div class="tabs">
      <div @click="clickQuestion" class="tabs__tab" :class="{active: activeTab}">
         Часто задаваемые вопросы
      </div>
      <div @click="clickInstruction" class="tabs__tab" :class="{active: !activeTab}">
         Инструкции
      </div>
   </div>
</template>

<script>
export default {
   name: "Tabs",
   props: [
      'activeTab',
   ],
   data() {
      return {}
   },
   methods: {
      clickQuestion() {
         this.$emit('clickQuestion')
      },
      clickInstruction() {
         this.$emit('clickInstruction')
      }
   }
}
</script>

<style lang="scss">

.tabs {
   font-size: 15px;
   display: flex;
   align-items: center;

   .tabs__tab {
      background-color: #fff;
      color: #ADADAD;
      display: flex;
      align-items: center;
      justify-content: center;
      border-bottom: 2px solid transparent;
      transition: .3s;
      cursor: pointer;
      height: 35px;
      margin-right: 35px;
      letter-spacing: 0.2px;
      font-weight: 600;

      &:last-child {
         margin-right: 0;
      }

      svg {
         fill: #333333;
         margin-right: 20px;
         transition: .3s;
      }
   }

   .tabs__tab.active {
      color: #333;
      border-bottom: 2px solid var(--mf-green);

      svg {
         fill: var(--mf-green);
      }
   }

}

</style>