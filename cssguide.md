# css Style Guide
css代码规范

## 组件开发细则
* 所有组件依赖[`pcadmin-base`](https://github.com/ksc-fx/pcadmin-base)。
* 组件内样式都包含到@{ksPrefix}XXX内
  ```css
    .@{ksPrefix}button {
        
    }
  ```
* 公用变量使用var.less中的变量
  ```css
    @import '~pcadmin-base/src/css/var.less';
    .@{ksPrefix}button {
        background-color: @dangerColor;
    }
  ```

* 公共基础css函数及常用类使用mixin.less
  ```css
    @import '~pcadmin-base/src/css/mixin.less';
    .@{ksPrefix}button {
        background-color: @dangerColor;
    }
  ```

* 私有函数写到私有化
  ```css
    // 函数begin
    .ks-button-default-function(@color) {
        background-color: @color;
        border-color: @color;
    }
    // 函数end

    .@{ksPrefix}button {
        .ks-button-primary-function(@FFFFFF);
    }
  ```

## 细则

* **使用四个空格**进行缩进。

  ```css
    .@{ksPrefix}button {
        background-color: @dangerColor;
    }
  ```

  * css规则一行一个，每一个以**分号';'**结尾。

  ```css
    .@{ksPrefix}button {
        height: 37px;
        width: 100px;
        background-color: @dangerColor;
    }
  ```

