### 小说类型列表接口

1、接口地址：/bookTypeList

2、参数

| 参数名 | 参数类型 | 是否必填 | 备注 |
| :--- | :--- | :--- | :--- |
| page | int | 否 | 页数，默认1 |
| limit | int | 否 | 一页几条，默认100 |

3、接口返回结构

```js
data: {
    "count": 全部小说类型数量
    "bookTypeList": [
        {
            "count(bookType)": 多少本这种类型的小说
            "bookType":"都市小说"
        },
        {
            "count(bookType)": 多少本这种类型的小说
            "bookType":"言情小说"
        }

    ]
}
```

4、接口返回例子

```js
{
  "code": 1000,
  "data": {
    "bookTypeList": [
      {
        "count(bookType)": 40,
        "bookType": "都市小说"
      },
      {
        "count(bookType)": 3,
        "bookType": "言情小说"
      }
    ],
    "count": 11
  },
  "msg": ""
}
```





