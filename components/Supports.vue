<template>
   <div class="supports">
      <h2>Не нашли что искали?</h2>
      <div class="supports__block">
         <a href="#">Онлайн-чат с поддержкой</a>
      </div>
   </div>
</template>

<script>
export default {
   name: "Supports"
}
</script>

<style lang="scss" scoped>
.supports {
   margin-bottom: 40px;

   h2 {
      font-size: 24px;
      margin-bottom: 16px;
   }

   &__block {
      background-color: #fff;
      padding: 19px 41px;

      a {
         display: inline-block;
         height: 24px;
         line-height: 24px;
         padding-left: 50px;
         color: var(--text-blue);
         font-size: 16px;
         background: #fff url('../assets/svg/Support-avatar_24.svg') 0 50% / contain no-repeat;
      }
   }
}

@media (max-width: 767px) {
   .supports__block {
      padding: 19px 17px;

      a {
         padding-left: 44px;
      }
   }
}

</style>