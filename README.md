# little-projects
calculator with php && html
<!DOCTYPE html>
<html>
<head>
	<title>Calculator</title>
</head>
<body>
	<form method="post">
		<input type="text" name="numero1">
		<select name="var">
			<option value="*">*</option>
			<option value="/">/</option>
			<option value="+">+</option>
			<option value="-">-</option>
		</select>
		
		<input type="text" name="numero2">
		<input type="submit" name="ação" value= "=" />	
<?php  


 //echo '<hr>';
 if($_POST['var']=='+' && isset($_POST['ação'])) {
			echo $_POST['numero1'] + $_POST['numero2'];
}
	else if($_POST['var']=='-' && isset($_POST['ação'])) {
			echo $_POST['numero1'] - $_POST['numero2'];
	}
		else if($_POST['var']=='*' && isset($_POST['ação'])) {
			echo $_POST['numero1'] * $_POST['numero2'];
		}	
			else if($_POST['var']=='/' && isset($_POST['ação'])) {
			echo $_POST['numero1'] / $_POST['numero2'];
			}				



?>



	</form>

</body>
</html>
