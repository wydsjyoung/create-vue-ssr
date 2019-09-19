<template>
    <div id="app">
        <header class="header">
            <nav class="inner">
            <router-link to="/" exact>
                <img class="logo" src="~public/logo-48.png" alt="zeromake">
            </router-link>
            <router-link to="/top">Top</router-link>
            <router-link to="/new">New</router-link>
            <a class="github" href="https://github.com/zeromake/my-vue-hackernews" target="_blank" rel="noopener">
              Built with zeromake
            </a>
            </nav>
        </header>
        <transition name="fade" mode="out-in">
            <router-view class="view"></router-view>
        </transition>
    </div>
</template>

<style lang="scss" scoped>
#app{
    width:100%;
    height:200px;
}
</style>
