# 运行生成文档的工具
```cmd
cnpm i docsify-cli -g
docsify serve
http://localhost:3000
```



npm i docsify-cli -g
# 列表

> 使用指南

```main.vue
import dxlist from './dxgj_uni/dx_list.vue'
Vue.component('dx_list',dxlist)
```

```xx.vue
<dx_list :title="'独行工匠'" :rtext="'介绍'" isjt="true"></dx_list>
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
num | 列元素宽度 |  -



# 单行输入框

> 使用指南

```main.vue
import dx_input from './components/dx_input.vue'
Vue.component('dx_input',dx_input)
```

```xx.vue
	<dx_input v-model="form.password" type="3" placeholder="密码" rightText="忘记密码" @rTextCabat="rTextCabat"></dx_input>
```
>参数说明
    
参数|说明|默认值
-|-|-
type | 类型 | 1文本  2数字  3密码 4搜索
rightText | 右边的文字 | -
rTextCabat | 点击右边区域 | -


# tab   切换

> 使用指南

```main.vue
import dx_tab from './components/dx_tab.vue'
Vue.component('dx_tab',dx_tab)
```

```xx.vue
			<dx_tab :title_d="title_d"></dx_tab>
            
            data(){
                return{
                    	title_d: [{
					name: "我发起的申诉",
					cls: "act",
					page: 1,
					date_df: [{
						id: 0
					}, {
						id: 1
					}]
				}, {
					name: "我收到的申诉",
					cls: "",
					page: 1,
					date_df: [{
						id: 3
					}, {
						id: 4
					}]
				}]
                }
            }
```
>参数说明
    
参数|说明|默认值
-|-|-
title_d | 数据 | -












