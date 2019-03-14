# lCalendar 

移动端日历选择框


## 修改优化：

为了项目功能，在原代码上扩展了一些方法，让其支持了日期区间选择、节假日是否可选、不可选日期等等功能，新增了两个回调方法。
 
 ## 演示


![lCalendar]()

#### Code DEMO
```javascript
let lcalendar = new lCalendar();
lCalendar.init({
	trigger: '#J_datetime',
	type: 'datetime',
	lcalendar: '1918-01-01,2018-01-01'
});
```
## 参数
| 参数        	| 说明           |
| ------------- |-------------|
|trigger		|[String], 文本框ID		|
| type          | [String]，类型：date/datetime/ym/time |
| lcalendar       | [String]：日期选择区间（最小日期和最大日期合并：2017-01-01,2017-02-01） | 
| dayDisabled       | [Array] 不可选择的日期 ['2018-02-10','2018-03-22','2018-04-23']      | 
| weekendDisabled  | [Boolean] true：周六日不可选择，false: 默认可选择 | 


## 回调

| 参数            | 说明          |
| -------------   |-------------|
| onConfirm   | [Function] 点击确定按钮 回调；参数为当前选择的日期格式为：2017-01-01 |
| onCancel | [Function] 点击取消按钮 回调； |
