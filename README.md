# my-first-web-static-app
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<script type="text/javascript">
var result_1;
//加法
function add() {
var a = getFirstNumber();
var b = getTwiceNumber();
var re = Number(a) + Number(b);
sendResult(re);
}
//減法
function subtract() {
var a = getFirstNumber();
var b = getTwiceNumber();
var re = a - b;
sendResult(re);
}
//乘法
function ride() {
var a = getFirstNumber();
var b = getTwiceNumber();
var re = a * b;
sendResult(re);
}
//除法
function devide() {
var a = getFirstNumber();
var b = getTwiceNumber();
var re = a / b;
sendResult(re);
}
//給p標簽傳值
function sendResult(result_1) {
var num = document.getElementById("result")
num.innerHTML = result_1;
}
//獲取第一位數字
function getFirstNumber() {
var firstNumber = document.getElementById("first").value;
return firstNumber;
}
//獲取第二位數字
function getTwiceNumber() {
var twiceNumber = document.getElementById("twice").value;
return twiceNumber;
}
</script>
</head>
<body>
<p>簡單計算器:</p>
<table border="1" style="position: center;">
<tr>
<td>第一個數：</td>
<td><input type="text" id="first" /></td>
</tr>
<tr>
<td>第二個數：</td>
<td><input type="text" id="twice" /></td>
</tr>
<tr>
<td colspan="2">&nbsp;
<button style="width: inherit" onclick="add()">+</button> &nbsp;
<button style="width: inherit" onclick="subtract()">-</button>
&nbsp;
<button style="width: inherit" onclick="ride()">*</button> &nbsp;
<button style="width: inherit" onclick="devide()">/</button>
</td>
</tr>
<tr>
<td colspan="2" rowspan="2">
<p id="result"></p>
</td>
</tr>
</table>

</body>
</html>
