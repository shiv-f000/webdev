# webdev
<!DOCTYPE html>
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" type="text/css" href="css/registrationstyle.css">
	<style type="text/css" ></style>
	<title>Regitration Form</title>
</head>
<body>
	<form>
		<div class="container">
			<h1>Book Rigistration form</h1>
			<p>Kindy fill the form</p>
			<!-- fields-->
			<label for="slno"><b>Slno</b></label>
			<input type="text" name="slno" id="slno" placeholder="slno" required/>

			<label for="booktitle"><b>Book Title</b></label>
			<input type="text" name="booktitle" id="booktitle" placeholder="Booktitle" required/>

			<label for="AuthoreName"><b>Authore Name</b></label>
			<input type="text" name="AuthoreName" id="AuthoreName" placeholder="Authore Name" required/>

			<label for="category"><b>Category</b></label>
			<select name="category" id="category">
			<option value="History">History</option>
			<option value="literature">Literature</option>
			<option value="art">Art</option></select>

			<label for="Price"><b>Price</b></label>
			<input type="number" name="price" id="price" placeholder="price" required/>

			<label for="yearofpublication"><b>Year of publication</b></label>
			<input type="month" name="yearofpublication" id="yearofpublication" min="1901-01" value="1901-01" required/>

			<button type="submit">Register</button>
		</div>
		<div id="languagediv">
			<h1>change language</h1>
			<button onclick="englishfont()">English Font</button>
			<button onclick="kannadafont()">kannada Font</button>
		</div>
	</form>

</body>
<script type="text/javascript">
	function kannadafont() {
		document.getElementById('booktitle').style.fontFamily = "myFirstFont";
		document.getElementById('AuthoreName').style.fontFamily = "myFirstFont";
		document.getElementById('category').style.fontFamily = "myFirstFont";
		document.getElementById('price').style.fontFamily = "myFirstFont";
		document.getElementById('yearofpublication').style.fontFamily = "myFirstFont";
	}

	function englishfont() {
		document.getElementById('booktitle').style.fontFamily = "monospace";
		document.getElementById('AuthoreName').style.fontFamily = "monospace";
		document.getElementById('category').style.fontFamily = "monospace";
		document.getElementById('price').style.fontFamily = "monospace";
		document.getElementById('yearofpublication').style.fontFamily = "monospace";
	}
</script>
</html>
