# Popup

弹窗
```js
import { $popup } from 'ml-ui'

Vue.prototype[$popup.name]= $popup
```
Demo1
```js
this.$popup.alert({message: '这是alert' }) 

this.$popup.confirm({ message: '这是confirm' }) 
```
Demo2 
```js
this.$popup({type:'alert',message: '这是alert' }) 

this.$popup({type:'confirm', message: '这是confirm' }) 
```
Props
| 参数          | 说明            | 类型            | 可选值                 | 默认值   |
|-------------  |---------------- |---------------- |---------------------- |-------- |
| title         | 标题   | String  | - | - |
| message         | 内容(支持html片段)   | String  | - | - |
| type         | 类型   | String  | alert、confirm  |  alert| 
| onConfirm        | 确定事件   | Function  | - |  -| 
| onClose         | 取消事件   | Function  | - | - |
| prevent    | 点击外层是否关闭   | Boolean  | true、false | false |
