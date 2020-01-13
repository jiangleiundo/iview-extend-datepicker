# iview-extend-datepicker
一个基于iview的日期组件扩展的日期组件, 基于iview 2.0版本

> 增加：季度选择 type=“quarter”
> 季度范围选择 type=“quarterrange”
> 月份范围选择 type=“monthrange”
>
> 若版本大于2.0 注意icon图标 date-pickers/picker.vue => 注意:239行方法iconType()

- 下载日期组件`date-pickers`将其放到compononents目录下，当然也可以放到其他目录。

- ```javascript
  // 引入组件，注册组件
  import DatePickers from '../../components/date-pickers'
  components: { DatePickers }
  ```

- ```html
  // 使用组件，使用方法可参考demo.vue
  <DatePickers type="monthrange" transfer format="yyyy-MM" v-model="month" placeholder="选择月份区间" style="width: 200px"></DatePickers>
  
  <DatePickers type="quarterrange" transfer format="yyyy-MM-dd" v-model="season" placeholder="选择季节区间" style="width: 200px"></DatePickers>
  ```

- type类型包括: [‘year’, ‘month’, ‘date’, ‘quarter’, ‘daterange’, ‘datetime’, ‘datetimerange’,‘monthrange’,‘quarterrange’]
  其他具体参数与iview相同
