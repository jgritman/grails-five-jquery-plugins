!SLIDE 

# Grails 1.x #

	@@@ xml

	<g:javascript library="prototype" />

!SLIDE

# Grails 2.0 #

	@@@ xml

	<g:javascript library="jquery" />

!SLIDE 

# some things you may have heard about jQuery... #

!SLIDE center

![](so-jquery2.png)

!SLIDE center

![](so-jquery1.png)

!SLIDE center

![](so-jquery3.png)

!SLIDE

# But seriously... #

  * jQuery solves many of the traditional problems involved in developing JavaScript intensive web applications

!SLIDE

# jQuery facts #

![](chuck_norris.jpg)

!SLIDE

 * Most popular JavaScript libary in use today
 * Used in 46% of top 10,000 websites
 * Embedded in many platforms (.NET, Grails)

!SLIDE

# So what is jQuery's magic formula? #


!SLIDE

# Selectors #

	@@@ javascript
		
		$('#myDiv') // id selector
		$('.myClass')  // class selctor
		$('div')  // type selector 

!SLIDE

# Selectors #

	@@@ javascript
		
		$(':input') // special selectors
		$('#main > div')  // child selctor
		$('#main form')  // descendant selector 

!SLIDE

# DOM Manipulation #

	@@@ javascript

		$('myDiv').addClass('myClass')
		$('myDiv').removeClass('myClass')

!SLIDE

# DOM Manipulation #

	@@@ javascript
		
		$('myDiv').show()
		$('myDiv').hide()

!SLIDE

# Event handling #

	@@@ javascript

		$(':button').click(function() {
			this.attr('disabled', 'disabled');
		});
		
!SLIDE

# Ajax support - Get data #

	@@@ javascript
		$.get('test.html', function(data) {
		  $('.result').html(data.title);
		});


!SLIDE

# Ajax support - load content #

	@@@ javascript

		// result of request will replace 
		// content of element with id result
		$('#result').load('test')

!SLIDE 		

# Grails ajax options #

 * g:remoteLink
 * g:formRemote
 * g:submitToRemote
 * Might work better than digging into jQuery depending on the task

