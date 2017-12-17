<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <!-- 引入样式 -->
  <link rel="stylesheet" href="https://unpkg.com/element-ui/lib/theme-chalk/index.css">
</head>
<body>
<div id="app">
<el-container style="height: 500px; border: 1px solid #eee">
  <el-aside width="200px" style="border: 1px solid #eee">2
    <el-menu>s</el-menu>
  </el-aside>
  <el-container>
    <el-header style="border: 1px solid #eee">s</el-header>
    <el-main style="border: 1px solid #eee">ddd</el-main>
  </el-container>
</el-container>
</div>
</body>
  <!-- 先引入 Vue -->
  <script src="https://unpkg.com/vue/dist/vue.js"></script>
  <!-- 引入组件库 -->
  <script src="https://unpkg.com/element-ui/lib/index.js"></script>
  <script>
    new Vue({
      el: '#app',
      data: {
        username : '',
        password : '',
        isload:false
      },
       methods: {
            open:function() {
                this.isload=true;
                setTimeout(function(){
                this.$alert('登录成功', '登录中');
                this.isload=false;
                 }.bind(this),2000)
            }
        }
    })
  </script>
</html>