# P2

### 题目一：

-请用原生`html` + `css` + `js`实现级联选择器，类似下图，样式不做要求。
![image](/image.png)

可以使用的 mock 数据

```javascript
[
  { id: 1, type: "province", displayName: "广东省", parentId: null },
  { id: 2, type: "province", displayName: "广西省", parentId: null },

  { id: 3, type: "city", displayName: "东莞市", parentId: 1 },
  { id: 4, type: "city", displayName: "广州市", parentId: 1 },
  { id: 5, type: "city", displayName: "深圳市", parentId: 1 },
  { id: 6, type: "city", displayName: "南宁", parentId: 2 },
  { id: 7, type: "city", displayName: "玉林", parentId: 2 },

  { id: 8, type: "area", displayName: "松山湖片区", parentId: 3 },
  { id: 9, type: "area", displayName: "东部产业园", parentId: 3 },
  { id: 10, type: "area", displayName: "滨海区", parentId: 3 },
  { id: 11, type: "area", displayName: "天河区", parentId: 4 },
  { id: 12, type: "area", displayName: "番禺区", parentId: 4 },
  { id: 13, type: "area", displayName: "宝安区", parentId: 5 },
  { id: 14, type: "area", displayName: "南山区", parentId: 5 },
  { id: 15, type: "area", displayName: "兴宁区", parentId: 6 },
  { id: 16, type: "area", displayName: "玉州区", parentId: 7 },
];
```

### 题目二：请用 `javascript` 实现一个函数 `parseUrl(url)`，将一段 url 字符串解析为 Object。

例如：

```js
parseUrl("http://www.bbkedu.com/product/list?id=123456&sort=discount#title");
```

期望结果：

```js
{
  protocol: "http",
  host: "www.bbkedu.com",
  path: "/product/list",
  params: {
    id: "12345",
    sort: "discount"
  },
  hash: "title"
}

```
