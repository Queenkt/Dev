<!DOCTYPE 
html>
 
<html lang="en">
 
<head>
 
<meta charset="UTF-8" />

<meta name="viewport" content="width=device-width, initial-scale=1.0" /> 
<title>REDACTR</title>
<link rel="stylesheet" href="./styles.css" />
</head>
<body>
<div class="container">
<h1 class="title">REDACTR</h1>
<p class="subtitle">
...SCRAMBLE SOME WORDS FROM A BODY OF TEXT CONTENT.
</p>
<form class="form_wrapper" id="myForm">
 
<div class="form_content">
 
<label class="form_label" for="content">Enter your content:</label>
 
<textarea
 
class="form_input_textarea"
 
id="content"
 
rows="5"
 
cols="40"
 
></textarea>
 
</div>
 
 
<div class="form_content">
 
<label class="form_label" for="redactWords"
 
>Words to be redacted (separated by spaces):</label
 
>
 
<input class="form_input" type="text" id="redactWords" />
 
</div>
 
 
 
<div class="form_content">
 
<label class="form_label" for="replacement"
 
>Choose a replacement:</label
 
>
 
<select class="form_input" id="replacement">
 
<option value="****">Asterisks</option>
 
<option value="????">Question Marks</option>
 
<option value="----">Dashes</option>
 
<option value="____">Underscores</option>
 
<option value="REDACTED">Custom Word (e.g., "REDACTED")</option>
 
</select>
 
</div>
 
 
 
<button class="redactButton" type="button" onclick="redactContent()">
 
Redact Now
 
</button>
 
 
 
<button class="resetButton" type="button" onclick="resetForm()">
 
Reset Form
 
</button>
 
</form>
 
 
 
<div class="redactContent" id="redactedContent">
 
<h2 class="redactedTitle">Redacted Content</h2>
 
<p id="redactedText" class="redactedText"></p>
 
<p class="statusTitle">Status:</p>
 
<p id="stats">
 
Words scanned: <span id="wordsScanned" class="counts">0</span>, Words
 
redacted: <span id="wordsRedacted" class="counts">0</span>, Characters
 
redacted: <span id="charactersRedacted" class="counts">0</span>, Time
 
taken: <span id="timeTaken" class="counts">0</span> seconds
 
</p>
 
</div>
 
</div>
 
<script src="contentRedactor.js"></script>
 
</body>
 
</html>
