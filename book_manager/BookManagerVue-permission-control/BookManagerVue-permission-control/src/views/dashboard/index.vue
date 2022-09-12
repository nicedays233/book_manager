<template>
  <div class="dashboard-container">
    <div title="欢迎页面" style="padding: 50px; overflow: hidden; color: #409eff;font: lighter 16px 'Lucida Sans Unicode';"
         data-options="iconCls:'icon-heart',plain:true">
        <b style="font-size: 36px; line-height: 30px; height: 30px;">欢迎使用图书管理系统</b>
        <p>内涵图书种类丰富，欢迎新老读者前来借阅。</p>
        <p>前端技术: HTML+CSS+JavaScript+Vue+Axios+ElementUI</p>
        <p>后端技术: Java+SpringBoot+MyBatis+MySQL</p>
    </div>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'id',
      'name',
      'roles'
    ])
  }
}
</script>
