﻿ajaxloader plugin requires jquery header file
Add Javascript Headers 
<head>
    <title></title>
    <script src="js/jquery-1.10.2.js" type="text/javascript"></script>
    <script src="js/ajaxloader.plugin.min.js" type="text/javascript"></script>  
</head>


Calling ajaxloader

    <script>
        $(document).ready(function () {
            $('#Div1').ajaxloader();
			//or
            $('.mydiv').ajaxloader();
			//or
            $('body').ajaxloader();
        });
    </script>

Plugin Options

	var loaderOptions={action:'show',loaderPosition:55,ajaxloaderImage:'js/loader/ajax-loader.gif'};
	if ajaxloaderImage width/height is not sufficient you can user {loaderWidth: 24, loaderHeight: 24} to loaderOptions
	$('body').ajaxloader(loaderOptions);

	for closing loader

	$('body').ajaxloader({action:'close'});