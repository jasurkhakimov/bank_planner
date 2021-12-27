<template>
  <div>
    <nav color="#fff" class="navigation">
        <div class="logo">
            IPAK YULI PROJECTS
        </div>

        <div class="links">
            <router-link active-class="active" :to="{name: 'main'}" class="link">
                Главная
            </router-link>
            <router-link active-class="active" :to="{name: 'projects'}" class="link">
                Проекты
            </router-link>
            <router-link active-class="active" :to="{name: 'boards'}" class="link">
                Доски
            </router-link>
        </div>
    </nav>
    <v-main>
        <router-view></router-view>
    </v-main>
  </div>
</template>

<script>
export default {};
</script>

<style lang='scss'>
.navigation {
    height: 56px;
    display: flex;
    align-items: center;
    padding: 4px 16px;
    border-bottom: 1px solid #eee !important;;
}


.links {
    display: flex;
    align-items: center;
    margin: 0 24px;
    gap: 12px;

    .link {
        padding: 8px 12px;
        background-color: #fff;
        border-radius: 5px;
        color: #191919;
        transition: 0.2s;

        &.active, &:hover {
            background-color: rgba(0,0,0,0.05);
            // color:#fff;
        }

        &:hover {
            background-color: rgba(0,0,0,0.05);
            // color:#fff;
        }


    }
}
</style>