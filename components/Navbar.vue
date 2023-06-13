<template>

<div class="container">    
   <nav class="navbar navbar-expand-sm navbar-dark bg-primary">
     <div class="container-fluid">
       <nuxt-link class="navbar-brand" to="/">
           <img src='img/icon96.svg' alt="" width="30" height="24">
       </nuxt-link>
       <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon"></span>
       </button>
       <div class="collapse navbar-collapse" id="navbarSupportedContent">
         <ul class="navbar-nav me-auto mb-2 mb-lg-0">
           <li class="nav-item">
             <nuxt-link class="nav-link active" aria-current="page" to="/home">Главная</nuxt-link>
           </li>
           <li class="nav-item">
             <nuxt-link class="nav-link" to="/">Link</nuxt-link>
           </li>
           <li class="nav-item dropdown">
             <nuxt-link class="nav-link dropdown-toggle" to="/" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
               Операции
             </nuxt-link>
             <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
               <li><nuxt-link class="dropdown-item" to="/sales">Записи из Sales</nuxt-link></li>
               <li><nuxt-link class="dropdown-item" to="/sp_get_talon">Информация по питанию</nuxt-link></li>
               <li><hr class="dropdown-divider"></li>
               <li><nuxt-link class="dropdown-item" to="/sp_accept_amcom_pay">Запись продаж</nuxt-link></li>
             </ul>
           </li>
         </ul>
         <form class="d-flex">
           <nav class="navbar navbar-dark bg-primary">
               <form class="container-fluid justify-content-start">
                 <nuxt-link to="/signin" class="btn btn-outline-light me-2">Вход</nuxt-link>
                 <nuxt-link to="/signout" class="btn btn-outline-light me-2">Выход</nuxt-link>
               </form>
             </nav>
         </form>
       </div>
     </div>
   </nav>
   </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
