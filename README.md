# jquery.bestupper
jQuery Upper Case Plugin


You must add jquery.min.js and jquery.bestupper.min.js in your code like this : 
```
<script src="https://code.jquery.com/jquery-2.2.4.min.js" type="text/javascript"> </script> 
<script src="jquery.bestupper.min.js" type="text/javascript"> </script>

<script type="text/javascript"> 
$(document).ready(function() { 
   $('.bestupper').bestupper(); 
}); 
</script>
```

Finally you must set class property to "bestupper" for each control

```
<input type="text" id="txtInput" class="bestupper" / > 
<textarea id="Textarea1" class="bestupper"></textarea >
```

There are tree option in this plugin. 
#### <i class="icon-pencil"></i> Option 1
#### ln:'en'

Default is 'en'. 

It is suport English and Turkish. 
If you are using Turkish keyboard you must set this option to 'tr' like this 
```
<script type="text/javascript">
$(document).ready(function() { 
   $('.bestupper').bestupper({ 
     ln: 'tr'
   }); 
}); 
</script>
```

#### <i class="icon-pencil"></i> Option 2
#### clear:true 
Default is true. 

This option clear whitespaces and try to upper (for pasted text) when exiting the control in blur event. 
If you don't want it ser clear option to false. If this option is false the bestupper plug in don't bind blur even to control. 

```
<script type="text/javascript">
$(document).ready(function() { 
   $('.bestupper').bestupper({ 
    clear:false
   }); 
}); 
</script>
```

#### <i class="icon-pencil"></i> Option 3
#### nospace:false 

Default is false. 

If you want to prevent enter space char you must use nospace:true 

```
<script type="text/javascript">
$(document).ready(function() { 
   $('.bestupper').bestupper({ 
    nospace:true
   }); 
}); 
</script>
```

You can use other ways to access control and apply bestupper method like this: 
```
<script type="text/javascript"> 
$(document).ready(function() { 
   $('#txtInput').bestupper(); 
}); 
</script>
```

This project developed by [Mustafa OZCAN](http://www.mustafaozcan.net)
