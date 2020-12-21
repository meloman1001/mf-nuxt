<template>
   <div class="copyright">
      6+© 2020 ПАО «МегаФон»<br>
      Продолжая использовать наш сайт, вы даете согласие на обработку файлов Cookies и
      других пользовательских данных, в соответствии с <a href="#">Политикой конфиденциальности.</a>
   </div>
</template>

<script>
export default {
   name: "Copyright"
}
</script>

<style lang="scss" scoped>
.copyright {
   font-size: 12px;
   line-height: 16px;
   max-width: 548px;

   a {
      color: var(--text-blue);
   }
}

@media (max-width: 767px) {
   .copyright {
      margin-bottom: 35px;
   }
}
</style>