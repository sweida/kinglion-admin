<template>
  <div>
    <headnav class="headnav"></headnav>
    <content class="content">
      <leftnav></leftnav>
      <router-view class="main-center scroll"/>
    </content>



  </div>
</template>

<script>
import headnav from '@/view/headnav'
import leftnav from '@/view/leftnav'
import '../style/common.css'

export default {
  name: 'app',
  components:{
    headnav,
    leftnav
  },
  data () {
    return {
    }
  },
}
</script>

<style lang="scss">
@import "../style/table.scss";
@import "../style/user.scss";
/*退出登录菜单样式*/
.el-dialog__title{
  font-size: 16px;
}
.el-menu--horizontal .el-submenu>.el-menu{
  top:60px;
  border-radius:0;
}
.el-submenu .el-menu-item{
  min-width: 150px;
}

</style>

