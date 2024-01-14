# ECharts-LIST
## 基于ECharts可视化记账清单小案例
## 一、需求分析
- 基本渲染

- 添加功能

- 删除功能

- 饼图渲染

## 二、思路分析

1.基本渲染  

- 立刻发送请求获取数据 created
- 拿到数据，存到data的响应式数据中
- 结合数据，进行渲染 v-for
- 消费统计  —> 计算属性

2.添加功能

- 收集表单数据 v-model，使用指令修饰符处理数据
- 给添加按钮注册点击事件，对输入的内容做非空判断，发送请求
- 请求成功后，对文本框内容进行清空
- 重新渲染列表

3.删除功能

- 注册点击事件，获取当前行的id
- 根据id发送删除请求
- 需要重新渲染

4.饼图渲染

- 初始化一个饼图 echarts.init(dom)    mounted钩子中渲染
- 根据数据试试更新饼图 echarts.setOptions({...})

## 三、实现效果

![Image text](https://github.com/wpper99/ECharts-LIST/blob/master/%E5%AE%9E%E7%8E%B0%E6%95%88%E6%9E%9C.png)
