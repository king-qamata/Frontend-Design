<template>
    <div class="container">
        <el-image src="icon.png" fit="scale-down" />
        <h2 class="subtitle">
            My luminous PWA project
        </h2>
        <div class="links">
            <a
                href="https://developers.google.com/web/progressive-web-apps"
                target="_blank"
                class="button--green"
            >
                Documentation
            </a>
            <router-link to="/albums" class="button--grey">
                Taylor Swift
            </router-link>
        </div>
    </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
    name: 'Home'
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.container {
    justify-content: center;
    align-items: center;
    text-align: center;
    .title {
        font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
            Roboto, 'Helvetica Neue', Arial, sans-serif;
        display: block;
        font-weight: 300;
        font-size: 100px;
        letter-spacing: 1px;
    }
    .subtitle {
        font-weight: 300;
        font-size: 42px;
        color: #526488;
        word-spacing: 5px;
    }
    .links {
        padding-top: 15px;
    }
    .button--green {
        display: inline-block;
        border-radius: 4px;
        border: 1px solid #3b8070;
        color: #3b8070;
        text-decoration: none;
        padding: 10px 30px;
    }
    .button--green:hover {
        color: #fff;
        background-color: #3b8070;
    }
    .button--grey {
        display: inline-block;
        border-radius: 4px;
        border: 1px solid #35495e;
        color: #35495e;
        text-decoration: none;
        padding: 10px 30px;
        margin-left: 15px;
    }
    .button--grey:hover {
        color: #fff;
        background-color: #35495e;
    }
}
</style>
