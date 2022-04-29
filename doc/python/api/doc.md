## 推荐的引入风格  

这一章里面API的定义已经展示了类的绝对位置，不过推荐使用下面引入风格：

```python
    from clicknium import clicknium as cc, selectorstore
```  

然后你就可以这样使用这个类：
```python
    clicknium.ie
    clicknium.chrome
    clicknium.find_element
``` 

特殊的枚举类(ClickType) 可以这样引入：  
`from clicknium.common.enums import ClickType`  

引入exception类（把SelectorUndefinedError替换为你真正需要的类名）：  
`from clicknium.common.models.exceptions import SelectorUndefinedError`

## API列表

