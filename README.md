ajaxForm
========

**ajaxForm** is a simple jQuery plugin to send ajax forms.
	
However, I must admit that the title is a bit misleading. The plugin itself does not *actually* perform server requests. It automatically sends form data to a specific javascript function. We can then take full advantage of jQuery built-in ajax functions to handle requests.

---

##Usage
	
Using ajaxForm is quite simple. Here's all the markup you need:
	

	<script src="js/jquery.min.js"></script>
	<script src="js/ajaxform.min.js"></script>
	
	<div class="ajaxform" data-action="myFunction" data-autoerase="true">
		<input type="text" name="field" placeholder="Type something">
		<button type="submit">OK!</button>
	</div>
	
	<script>
		$(function() {
			$(".ajaxform").ajaxForm();
		});
		
		var myFunction = function(data) {
			alert(data.field);
		}
	</script>
	
---
## Download
[On my website](http://www.arthurcamara.com/ajaxform) or on [GitHub](https://github.com/arthurcamara1/ajaxForm)

---
#### About Me
My name is Arthur Câmara. I’m a web designer and developer from Belo Horizonte, Brazil. [Check out my website](http://www.arthurcamara.com) or [send me an email](mailto:arthurcamara@gmail.com)


