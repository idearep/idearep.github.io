---
redirect_to: "http://madsbuch.com"
---

<html>
	<head>
		<title>Redirect to madsbuch.com</title>
	</head>
	<body>
		<p>
			This site has been moved to <span id="to"></span>
		</p>
		<script>
			var queryString = window.location.pathname + window.location.search + window.location.hash;
			var url = "http://madsbuch.com" + queryString;
			document.getElementById("to").innerHTML = "<a href=\"" + url + "\">" + url + "</a>";
			window.location = url;
		</script>
	</body>
</html>
