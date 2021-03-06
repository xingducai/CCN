总操作流程：
- 1、[删除内容和文件](#vue.js-01)
- 2、[创建文件](#vue.js-02)
- 3、[修改路由](#vue.js-03)
- 4、[看效果](#vue.js-04)

***

# <a name="vue.js-01" href="#" >删除内容和文件</a>

> 1、创建vue项目

[![](https://img.shields.io/badge/参考文献-Vue.js之下载安装与项目的搭建-yellow.svg "参考文献 Vue.js之下载安装与项目的搭建")](https://github.com/OurNotes/CCN/blob/master/2.%E5%89%8D%E7%AB%AF/3.vue/2.vue.js%E4%B9%8B%E5%AD%A6%E4%B9%A0/1-Vue.js%E4%B9%8B%E4%B8%8B%E8%BD%BD%E5%AE%89%E8%A3%85%E4%B8%8E%E9%A1%B9%E7%9B%AE%E7%9A%84%E6%90%AD%E5%BB%BA.md)

`注意：服务器启动后不用关掉，代码修改后，直接可以在http://localhost:8080/查看`

> 2、删除App.vue文件的内容

- 改后效果
```html
<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>

</style>

```

> 3、删除vue项目文件

![](image/3-1.png)


# <a name="vue.js-02" href="#" >创建文件</a>

> 1、创建新的vue文件

![](image/3-2.png)

> 2、创建Table.vue
```html
<template>
  <div>{{test}}</div>
</template>
<script>
export default {
  name: 'Table',
  data () {
    return {
      test: '1111111111111111'
    }
  }
}
</script>

<style scoped>

</style>
```

> 3、修改HelloWorld.vue
```html
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style scoped>

</style>

```

# <a name="vue.js-03" href="#" >修改路由</a>

![](image/3-3.png)

```js
import Vue from 'vue'
import Router from 'vue-router'
import HelloWorld from '@/components/HelloWorld'
import Table from '@/components/page/table'

Vue.use(Router)

export default new Router({
  routes: [
    {
      path: '/',
      name: 'HelloWorld',
      component: HelloWorld
    },
    {
      path: '/Table',
      name: 'Table',
      component: Table
    }
  ]
})
```

# <a name="vue.js-04" href="#" >看效果</a>

```
http://localhost:8080/#/Table
```



