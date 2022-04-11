<template>
  <div id="app">
    <v-app>
      <!-- 상단 툴바 -->
            <AppToolbar />

            <!-- 메인 섹션 -->
            <v-main>
                <MainList />

                    <!-- 일기 작성칸 -->
                    <v-container>
                        <WriteField />
                    </v-container>
            </v-main>


            <!-- 푸터 영역 -->
            <v-footer color="info lighten-2" dark>
                <div class="mx-auto">
                    <small>Copyright &copy; 2022 송민주. m1njuju , Ltd. All Rights Reserved</small>
                </div>
            </v-footer>
    </v-app>
    <router-view/>
  </div>
</template>

<script>
import AppToolbar from './components/AppToolbar.vue'
import MainList from './components/MainList.vue'
import WriteField from './components/WriteField.vue'


export default {
  name:'App',
  components: {
    AppToolbar,
    MainList,
    WriteField
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
