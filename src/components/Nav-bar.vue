<script setup>
import Searcher from './Searcher.vue'
import Setting from './Buttons/Setting.vue'
import Notification from './Buttons/Notification.vue'
import Chat from './Buttons/Chat.vue'
import Promo from './Buttons/Promo.vue'
import Profile from './Profile.vue'
import Burger from './Burger.vue'
import Breadcrumb from './breadcrumb.vue'

</script>

<template>
<nav class="nav-bar">
    <div class="navigation">
        <Burger/>
        <img class="logo" src="/logo.png" alt="logo">
    </div>
    <div class="searcher hide">
        <Searcher/>
        <Setting class="button-nav"/>
    </div>
    <div class="options">
        <div class="items-options">
            <Notification class="button-nav"/>
            <Chat class="button-nav"/>
            <Promo class="button-nav"/>

        </div>
        <hr class="separator hide">
        <Profile class="button-nav"/>
    </div>
   
</nav>
<Breadcrumb/>
</template>

<style scoped>
.nav-bar{
    background-color: #24292E;
    height: 2.65vw;
    padding: 1.67vw 2.81vw 1.67vw 1.72vw;
    display: flex;
    
}

.logo{
    height: 2.65vw;
}

.navigation{
    margin-right: 5.79vw;

    display: flex;
    align-items: center;
}

.searcher{
    margin-right: 12.7vw;
    width: 43.13vw;
    display: flex;
    align-items: center;
    gap: 1.04vw;
}

.options{
    display: flex;
    align-items: center;
    gap: 1.88vw;
}

.items-options{
    display: flex;
    gap: 0.99vw;

}

.separator{
    rotate: 180deg;
    height: 2.92vw;
    border: 1px solid rgba(247, 247, 247, 0.03);
    margin: 0;
}

.button-nav{
    cursor: pointer;
}
</style>