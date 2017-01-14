

## 使用示例

```javascript
var selectContainer = $("#appTypeSelector");
for(var i=0,len=data.length; i<len; i++){
  var cachedAppType = data[i];
  var appType = cachedAppType['appType'];

  var $option = $('<option data-spellHead="'+cachedAppType['appSpellHead']+'" data-spell="'+cachedAppType['appSpell']+'" data-value="'+appType+'" value="'+appType+'">'+cachedAppType['appName']+'</option>');
  var imgIcon = basePath+"/images/statistics/icon.png";
  $option.data("imgURI",imgIcon);
  selectContainer.append($option);
}

selectContainer.comboSelect();
```



## 图示：

![](https://raw.githubusercontent.com/webinglin/combo-select/master/qq.png)