<template>
   <header>
      <div class="wrapper">
         <a href="#" class="header__logo"></a>
         <h6 class="header__phone">
            <a href="tel:8 800 55-00-001">8 800 55-00-001</a>
         </h6>
         <a class="header__phone-mobile" href="tel:8 800 55-00-001">
            <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 32 32">
               <defs></defs>
               <g transform="translate(-4 -4)">
                  <path class="a" d="M17,6V4A19,19,0,0,1,36,23H34A17,17,0,0,0,17,6Z"/>
                  <path class="a" d="M17,18V16a7,7,0,0,1,7,7H22A5,5,0,0,0,17,18Z"/>
                  <path class="a" d="M17,12V10A13,13,0,0,1,30,23H28A11,11,0,0,0,17,12Z"/>
                  <path class="a"
                        d="M21.48,36h1L26,32.44l-6.83-6.83-2.78,2.78a12.52,12.52,0,0,1-4.94-4.78l2.78-2.78L7.56,14,4,17.56v1A17.71,17.71,0,0,0,21.48,36ZM6,18.38l1.56-1.56,3.85,4L9,23.23l.33.65a14.79,14.79,0,0,0,6.79,6.63l.65.33,2.4-2.4,4,4L21.62,34h-.14A15.6,15.6,0,0,1,6,18.52Z"/>
               </g>
            </svg>
         </a>
      </div>
   </header>
</template>

<script>
export default {
   name: "Header"
}
</script>

<style lang="scss" scoped>
header {
   background-color: #fff;
   position: relative;
   box-shadow: 0 0 15px #00000026;

   .wrapper {
      height: 70px;
      display: flex;
      align-items: center;
      justify-content: space-between;
   }

   .header__logo {
      max-height: 32px;
      max-width: 181px;
      width: 100%;
      height: 100%;
      background: url('../assets/svg/mf_logo_full.svg') center / contain no-repeat;
      fill: black;
   }

   .header__phone a {
      font-weight: 500;
   }

   .header__phone a:hover {
      color: inherit;
   }

   a.header__phone-mobile {
      display: none;
   }

}

@media (max-width: 767px) {
   header {

      .wrapper {
         height: 64px;
      }

      .header__logo {
         max-height: 24px;
         max-width: 135px;
      }

      h6 {
         display: none;
      }

      a.header__phone-mobile {
         display: block;
         width: 32px;
         height: 32px;
         margin-right: 18px;

         svg {
            display: block;
         }
      }

   }
}
</style>