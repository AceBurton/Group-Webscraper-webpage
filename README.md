# Group-Webscraper-webpage
<!DOCTYPE.HTML>
<html>
<link rel="stylesheet" type="text/css" href="main.css">
	<head>
	<h1>
		<Strong>Group Webscrapper Project </br> <i>Magic Happens</i></strong>
	</h1>
	</head>
	<body>
	<h2>
		<strong>Performed by Ace Burton</strong>
	</h2>
	<p>
		I worked on the Magic Happens step of the code, so once we get a user entry from the GUI section of are code, We then actually scrape the webpage for his Adam Drivers acting credits.
	</p>
	
	<p>
		This is the specific part we want to scrape:
	</p>
	<img src = img7.png>
	<p>
		First it takes the url the User submitted and gets the full HTML from the webpage.
	</p>
	<img src = img1.png>
	<p>
		It is then added to beautiful soup.
	</p>
	<img src = img2.png>
	<p>
		It then finds the div "filmo-head-actor" to just the HTML of that section of the full page.
	</p>
	<img src = img3.png>
	<p>
		It gives us this
	</p>
	<img src = img8.png>
	<p>
		Then it has to remove some stuff. We don't want either of the "span" tags, or the "a" tag. It also isolates just the text. Then we don't want the perentacies so it removes both of those. We are left with just the number of credits followed by the word "credits".
	</p>
	<img src = img4.png>
	<p>
		It removes all of this:
	</p>
	<img src = img10.jpg>
	<p>
		Now that it has the exact string we want we need to get it to only send a message when the code is updated. 	
	</p>
	<p>
		It first compares the number of credits he has after it is run to before to see if it has changed. 	
	</p>
	<img src = img5.png>
	<p>
		If it has changed then it creates the output "Adam Driver now has _ Credits". So some static text we wrote for context, and the string. It sends that all of to the next step to be sent via SMS through Twilio to the user.
	</p>
	<img src = img6.png>

	</body>
</html>
