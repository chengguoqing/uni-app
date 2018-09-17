# 列表

> 使用指南

```main.vue
import dxlist from './dxgj_uni/dx-list.vue'
Vue.component('dx-list',dxlist)
```

```xx.vue
<dx-list :title="'独行工匠'" :rtext="'介绍'" isjt="true"></dx-list>
```
>参数说明
    
参数|说明|默认值
-|-|-
title | 标题 | 独行工匠
rtext | 右边介绍 | 介绍
isjt | 右边的箭头 | false


# Layout 布局
> 使用指南

```main.vue
 import dx_row from './dxgj_uni/dx_row.vue'
 import dx_col from './dxgj_uni/dx_col.vue'
 
 Vue.component('dx_row',dx_row)
Vue.component('dx_col',dx_col)
```

```xx.vue
<dx_row gutter="20">
              <dx_col  :num="6">333</dx_col>
              <dx_col  :num="8">333</dx_col>
              <dx_col  :num="10">333</dx_col>
        </dx_row>
```


>参数说明
    
参数|说明|默认值
-|-|-
gutter | 间距 | dx_col也可以加
num | - | 列元素宽度