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
	
	<link href="http://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
	
	<link rel="stylesheet" type="text/css" href="https://ffirsttname.github.io/copy-excal/css/demo.css">
	<link rel="stylesheet" href="https://ffirsttname.github.io/copy-excal/dist/excel-bootstrap-table-filter-style.css" />
	
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

<h3>自動捲動+標題置頂（選擇性）</h3>

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
