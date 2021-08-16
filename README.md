# copy-excal
只作外連用，不提供任何回答
<br/>
<h3>演示</h3>

![image](https://user-images.githubusercontent.com/87819805/126663777-3eb0cd90-2458-44a4-b1d0-b549355d382c.png)

<h3>源碼HTML（外連）</h3>

```
<!DOCTYPE html>
<html lang="zh">
<head>
	<meta charset="UTF-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1"> 
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>仿Excel樣式的jquery表格排序外掛程式</title>
	
	<link href="http://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet"	
	<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/gh/ffirsttname/copy-excal/css/demo.css">
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/ffirsttname/copy-excal/dist/excel-bootstrap-table-filter-style.css" />
	<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
	<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/ffirsttname/copy-excal/dist/excel-bootstrap-table-filter-bundle.js"></script>
	
</head>
<body>

<div class="container">
  <div class="row">
    <div class="col-md-12">
      <h2>Table 1</h2>
      <table id="table" class="table table-bordered table-intel">
        <thead>
          <tr>
            <th class="filter">Animal</th>
            <th class="filter">Class</th>
            <th class="filter">Collective Noun</th>
            <th class="filter">A Number</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Bear</td>
            <td>Mammal</td>
            <td>Sleuth</td>
            <td>1</td>
          </tr>
          <tr>
            <td>Ant</td>
            <td>Insect</td>
            <td>Army</td>
            <td>2</td>
          </tr>
          <tr>
            <td>Salamander</td>
            <td>Amphibian</td>
            <td>Congress</td>
            <td>3</td>
          </tr>
          <tr>
            <td>Owl</td>
            <td>Bird</td>
            <td>Parliament</td>
            <td>4</td>
          </tr>
          <tr>
            <td>Frog</td>
            <td>Amphibian</td>
            <td>Army</td>
            <td>5</td>
          </tr>
          <tr>
            <td>Shark</td>
            <td>Fish</td>
            <td>Gam</td>
            <td>6</td>
          </tr>
          <tr>
            <td>Kookaburra</td>
            <td>Bird</td>
            <td>Cackle</td>
            <td>7</td>
          </tr>
          <tr>
            <td>Crow</td>
            <td>Bird</td>
            <td>Murder</td>
            <td>8</td>
          </tr>
          <tr>
            <td>Elephant</td>
            <td>Mammal</td>
            <td>Herd</td>
            <td>9</td>
          </tr>
          <tr>
            <td>Barracude</td>
            <td>Fish</td>
            <td>Grist</td>
            <td>10</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
  <div class="row">
    <div class="col-md-12">
      <h2>Table 2</h2>
      <table id="table2" class="table table-bordered table-intel">
        <thead>
          <tr>
            <th class="filter">Animal</th>
            <th class="filter">Class</th>
            <th class="filter">Collective Noun</th>
            <th class="filter">A Number</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Bear</td>
            <td>Mammal</td>
            <td>Sleuth</td>
            <td>1</td>
          </tr>
          <tr>
            <td>Ant</td>
            <td>Insect</td>
            <td>Army</td>
            <td>2</td>
          </tr>
          <tr>
            <td>Salamander</td>
            <td>Amphibian</td>
            <td>Congress</td>
            <td>3</td>
          </tr>
          <tr>
            <td>Owl</td>
            <td>Bird</td>
            <td>Parliament</td>
            <td>4</td>
          </tr>
          <tr>
            <td>Frog</td>
            <td>Amphibian</td>
            <td>Army</td>
            <td>5</td>
          </tr>
          <tr>
            <td>Shark</td>
            <td>Fish</td>
            <td>Gam</td>
            <td>6</td>
          </tr>
          <tr>
            <td>Kookaburra</td>
            <td>Bird</td>
            <td>Cackle</td>
            <td>7</td>
          </tr>
          <tr>
            <td>Crow</td>
            <td>Bird</td>
            <td>Murder</td>
            <td>8</td>
          </tr>
          <tr>
            <td>Elephant</td>
            <td>Mammal</td>
            <td>Herd</td>
            <td>9</td>
          </tr>
          <tr>
            <td>Barracude</td>
            <td>Fish</td>
            <td>Grist</td>
            <td>10</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
  <div class="row">
    <div class="col-md-12">
      <h2>Table 3</h2>
      <p>姓名欄位只提供搜索，不帶過濾和排序</p>
      <table id="table3" class="table table-bordered table-intel">
        <thead>
          <tr>
            <th class="filter">編號</th>
            <th class="no-sort no-filter">姓名</th>
            <th class="filter">成績</th>
          </tr >
        </thead>
        <tbody>
        	<tr>
        		<td>1</td>
        		<td>張三</td>
        		<td>68</td>
        	</tr>
        	<tr>
        		<td>2</td>
        		<td>李四</td>
        		<td>75</td>
        	</tr>
        	<tr>
        		<td>3</td>
        		<td>王五</td>
        		<td>86</td>
        	</tr>
        	<tr>
        		<td>4</td>
        		<td>趙六</td>
        		<td>76</td>
        	</tr>
        	<tr>
        		<td>5</td>
        		<td>韓七</td>
        		<td>95</td>
        	</tr>
        </tbody>
      </table>
    </div>
  </div>
</div>


<script type="text/javascript" src="https://ffirsttname.github.io/copy-excal/js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="https://ffirsttname.github.io/copy-excal/dist/excel-bootstrap-table-filter-bundle.js"></script>
<script type="text/javascript">
$(function () {
  $('#table').excelTableFilter({
	'captions':{ a_to_z: '昇冪排列', z_to_a: '降冪排列', search: '搜索', select_all: '全部選擇' }
  });
  $('#table2').excelTableFilter({
	'captions':{ a_to_z: '昇冪排列', z_to_a: '降冪排列', search: '搜索', select_all: '全部選擇' }
  });
  $('#table3').excelTableFilter({
		'captions':{ a_to_z: '昇冪排列', z_to_a: '降冪排列', search: '搜索', select_all: '全部選擇' }
  });
});
</script>

</body>
</html>

```

<h3>修改表格不要搜索/篩選/排序 條改搜索嘅名等 修改篩選高度</h3>

修改表格不要搜索/篩選/排序<br/>
可以將原來```<th class="filter">姓名</th>```中的filter條改

例如原本
```<th class="filter">姓名</th>```改為```<th class="no-sort no-filter">姓名</th>>```

```no-sort```代表不排序
```no-filter```代表不篩選
```no-search```代表不搜索

修改搜索嘅名等（原文已添加）
```
<script type="text/javascript">
$(function () {
  $('#table').excelTableFilter({
	'captions':{ a_to_z: '昇冪排列', z_to_a: '降冪排列', search: '搜索', select_all: '全部選擇' }
});
</script>
```

在<style>和</style>之間加入以下程式碼，200px就係佢個高度，原本預設係400px

```
.checkbox-container{
  max-height:200px;
}
```

<h3>自動捲動+標題置頂（選擇性）需要加多個搜索+置頂 <a href="#加多一個搜索框" rel="nofollow">按我</a></h3>

```
<!--多左出來會自動捲動+標題置頂-->
<style>
div.col-md-12{
 overflow:auto;
 width:100%;
 height:500px; /* 固定高度 */
}
  
thead tr th {
 position:sticky;
 top:0; /* 列首永遠固定於上 */

}
  
th:first-child{
 z-index:2;
}
  
/*<br/>先會換行*/
#table * { white-space: pre; }
</style>
<!--多左出來會自動捲動-->
```

<h3>加多一個搜索框</h3>
找到

```
<h2>Table 1</h2>
```

下面添加 
data-table同table的class要一樣

```
<div class="tablesearch">搜尋：<input type="search" class="light-table-filter" data-table="table table-bordered table-intel" placeholder="請輸入關鍵字"></div>

```

之後<script> 與 </script>添加以下程式碼

```
<!--增加多一個資料搜尋-->
<script>
  (function(document) {
  'use strict';

  // 建立 LightTableFilter
  var LightTableFilter = (function(Arr) {

    var _input;

    // 資料輸入事件處理函數
    function _onInputEvent(e) {
      _input = e.target;
      var tables = document.getElementsByClassName(_input.getAttribute('data-table'));
      Arr.forEach.call(tables, function(table) {
        Arr.forEach.call(table.tBodies, function(tbody) {
          Arr.forEach.call(tbody.rows, _filter);
        });
      });
    }

    // 資料篩選函數，顯示包含關鍵字的列，其餘隱藏
    function _filter(row) {
      var text = row.textContent.toLowerCase(), val = _input.value.toLowerCase();
      row.style.display = text.indexOf(val) === -1 ? 'none' : 'table-row';
    }

    return {
      // 初始化函數
      init: function() {
        var inputs = document.getElementsByClassName('light-table-filter');
        Arr.forEach.call(inputs, function(input) {
          input.oninput = _onInputEvent;
        });
      }
    };
  })(Array.prototype);

  // 網頁載入完成後，啟動 LightTableFilter
  document.addEventListener('readystatechange', function() {
    if (document.readyState === 'complete') {
      LightTableFilter.init();
    }
  });

})(document);
  </script>
<!--增加多一個資料搜尋-->
```


<h3>多左出來會自動捲動+搜索同標題置頂（選擇性）</h3>

```
<!--多左出來會自動捲動-->
<style>
div.col-md-12{
 overflow:auto;
 width:100%;
 height:500px; /* 固定高度 */
}
  
thead tr,thead th, div.tablesearch{
 position:sticky;
 top:0; /* 列首永遠固定於上 */
}
  
thead tr,thead th {
 top:29.3px; 

}

/*搜索欄樣式+不換行*/
div.tablesearch{background-color: #DDDDDD;border:1px solid #AAAAAA;width:200px;white-space: pre;padding-left:5px;padding-right:45px}
.tablesearch .light-table-filter{width:100%;border: 1px solid;}
  
th:first-child{
 z-index:2;
}
  
/*<br/>先會換行*/
#table * { white-space: pre; }
</style>
<!--多左出來會自動捲動-->
```


