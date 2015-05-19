# ui-panel

---

* *组件说明：* 区块面板基础UI组件；
* *依赖CSS：* `_ui-panel.scss`、`_ui-lineList.scss`；

---

## 默认面板区块 `@base`

````html
<div class="ui-panel">
    <div class="ui-panel__hd">
        <i class="ui-panel__ico"></i>
        <h3 class="ui-panel__tit">区块面板标题</h3>
        <span class="ui-panel__meta">额外文本</span>
        <div class="ui-panel__more ui-lineList">
            <a href="#">链接1</a>
            <a href="#">链接2</a>
            <a href="#">更多»</a>
        </div>
    </div>
    <div class="ui-panel__bd">
        <p>ui-panel 默认无内边距</p>
        <p>区块内容区块内容区块内容区块内容区块内容区块内容区块内容区块内容区块内容</p>
    </div>
</div>
````

## 带边框的面板区块 `@extend: .ext-border`

````html
<div class="ui-panel ext-border">
    <div class="ui-panel__hd">
        <i class="ui-panel__ico"></i>
        <h3 class="ui-panel__tit">区块面板标题</h3>
        <span class="ui-panel__meta">额外文本</span>
        <div class="ui-panel__more ui-lineList">
            <a href="#">链接1</a>
            <a href="#">链接2</a>
            <a href="#">更多»</a>
        </div>
    </div>
    <div class="ui-panel__bd">
        <p>ext-border 默认带内边距</p>
        <p>区块内容区块内容区块内容区块内容区块内容区块内容区块内容区块内容区块内容</p>
    </div>
</div>
````
<br/>

````html
<div class="ui-panel ext-border">
    <div class="ui-panel__hd">
        <i class="ui-panel__ico"></i>
        <h3 class="ui-panel__tit">没有内容</h3>
        <span class="ui-panel__meta">额外文本</span>
        <div class="ui-panel__more ui-lineList">
            <a href="#">链接1</a>
            <a href="#">链接2</a>
            <a href="#">更多»</a>
        </div>
    </div>
</div>
````

## 弹窗型面板区块 `@extend: .ext-pop`

````html
<div class="ui-panel ext-pop">
    <div class="ui-panel__hd">
        <h3 class="ui-panel__tit">弹窗面板标题</h3>
        <span class="ui-panel__meta">额外文本</span>
        <div class="ui-panel__more">
            <a href="###" class="ui-panel__close" data-role="pop-close-btn">&times;</a>
        </div>
    </div>
    <div class="ui-panel__bd">
        还可以拓展为弹窗哦
    </div>
</div>
````

## 实际应用例子 `.ext-zoneCol`

````html
<div class="ui-panel ext-zoneCol">
    <div class="ui-panel__hd">
        <h3 class="ui-panel__tit">论坛热帖</h3>
        <span class="ui-panel__meta">额外文本</span>
        <div class="ui-panel__more ui-lineList">
            <a href="#">链接1</a>
            <a href="#">链接2</a>
            <a href="#">更多»</a>
        </div>
    </div>
    <div class="ui-panel__bd">
        <p>扩展类示例</p>
        <p>区块内容区块内容区块内容区块内容区块内容区块内容区块内容区块内容区块内容</p>
    </div>
</div>
````

````css
.ui-panel.ext-zoneCol .ui-panel__hd {
    height: 20px;
    line-height: 20px;
    border-bottom: 1px solid #eaeaea;
}
.ui-panel.ext-zoneCol .ui-panel__tit {
    padding-bottom: 7px;
    border-bottom: 2px solid #3a6ecc;
    font-size: 18px;
}
````

## History

### 1.0.0 *2014-09-05*

`NEW` ui-panel First version.

### 1.1.0 *2015-02-12*

`IMPROVED` 模块命名规范更新，统一使用`ui`前缀；

`IMPROVED` 结构、细节优化完善；


### 1.2.0 *2015-04-08*

`IMPROVED` 命名优化，拓展类使用`ext-`前缀代替双中划线；

### 1.3.0 *2015-05-16*

`NEW` 组件改名`ui-panel`；

`NEW` 增加依赖组件`ui-lineList`；

