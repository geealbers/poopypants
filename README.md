poopypants
==========

**The impromptu code lesson that made my 8yo say "code is cool" for the first time**

Let's say we wanted to make a webpage that said "Hello world!" on it. We need to tell the computer to do this, but in what language? We could try plain English: 

```
Computer, write "Hello world!" on a webpage.
```

But the computer's not going to understand that language. Just like some people speak English, some speak Spanish, and some speak any number of other languages; computers speak their own languages. The language we would use to write "Hello wolrd!" on a webpage actually looks like this:

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>My Webpage</title>
</head>
<body>
	<p>Hello world!</p>
</body>
</html>
```
Open the `poopypants.html` file in a browser to see. It works! And even though the language we had to speak to the computer seems pretty complicated and hard to read ourselves, the more we learn how to speak it, the more we can make the computer do.

Maybe we want the "Hello world!" to be bigger. See those p's in brackets around our "Hello world!" in the code? Those p's stand for paragraph. Let's change them to h1's, which stands for Heading #1 (the biggest of six possible headings), and see what happens:

```html
  <h1>Hello world!</h1>
```  

Bigger! And how about a different color? That we can do by telling the computer a style to use. There are a couple ways to do this, but for simplicity, we can do it right next to those h1 tags:

```html
  <h1 style="color:red;">Hello world!</h1>
```

"But what," my son asked, "if we want it to say 'I am a poopy pants'"?

Good question! We could just replace the words "Hello world!" with "I am a poopy pants!" but better yet:

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>My Webpage</title>
	<script>
		function myPants() {
			alert("I am a poopy pants!");
			}
	</script>
</head>
<body>
	<h1 style="color:red" onclick="myPants()">Hello world!</h1>
</body>
</html>
```

Or this is the one that really won him over:

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>My Webpage</title>
	<script>
		function myPants() {
			document.getElementById("pants").style.display="inline";
			}
	</script>
</head>
<body>
	<h1 style="color:red" onclick="myPants()">Daddy <span id="pants" style="display:none">is a poopy pants!</span></h1>
</body>
</html>
```

