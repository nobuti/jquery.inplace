Small plugin to add "edit-in-place" funcionality.


## Example of use

	var options = {
		event:'editEvent', 	// triggered event
		key: 'cmd',			// key + intro combination key (CMD or CTRL)
		class: 'rollover'	// class to control hover effect
	}
	
	$(document).ready(function() {
		  
		$(".editable")
	      	.inplace({
	      		event:'editEvent',
	      		key: 'cmd',
	      		class: 'rollover'
	      	})
	      	.on('editEvent', function(e){
	      		console.log('trigger event: save content for example');
			});
	});

You should now be able to edit all objects of class 'editable' in place.