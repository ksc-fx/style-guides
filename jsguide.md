# JavaScript Style Guide
js代码规范基础是
[`standard`](https://github.com/standard/standard/blob/master/docs/RULES-zhcn.md)
部分不符合活需要注意的使用规则见下面细则

## 组件开发细则
* 所有组件所需的js工具类依赖[`pcadmin-base`](https://github.com/ksc-fx/pcadmin-base)。


## 细则

* **使用四个空格**进行缩进。

  ```js
    function hello (name) {
        console.log('hi', name);
    };
  ```
* 每一行语句以**分号';'**结束。

    ```js
    function hello (name) {
        console.log('hi', name);
    };
    ```