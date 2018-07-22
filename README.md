# antd-mobile-area-data

## 安装

```bash
$ yarn add antd-mobile-area-data
```

## 使用

```js
import { pc, pca, pcas } from 'antd-mobile-area-data'
```

- pc：二级联动
- pca：三级联动
- pcas：四级联动

## label == value

```js
function handleData(datas) {
  datas.forEach(item => {
    item.value = item.label
    if (item.children) {
      this.handleData(item.children)
    }
  })
}
```
