Template Pack Guidelines

Image Buttons
-------------
Use the supplied template file (it should be in the images folder) to create site buttons for the localized social bookmarking services.
Make sure that the file name of your button is the same with the file name in your XML file.
Once you have finished your buttons place them in the image folder.

Site Definitions
----------------
Every site is defined in a XML file named as sites_XX.xml where XX shoud be the ISO country code for the language that you are working on.
Open the sites_template.xml file and edit it in your favourite text editor.
For each site that you want to include add the following code with your changes:
	<site>
    <name>Site_Name</name>
	<url>http://siteurl.com/post.html.php?url={link}&amp;title={title}</url>
	<img>image_file</img>
	<key>site_key</key>
    </site>
	
where:
	site_name should be the name of the site (like Digg, Del.ici.ous)
	
	image_file should be the file name of the button that you have created in the images folder.
	
	site_key should be a *unique* word to identify your site. To avoid having the same site_key
				in different language packs, please append an underscore followed by the language
				code. For instance if you are creating a german pack and you want to include 
				Mister Wong then please enter 'misterwong_ge' (without the quotes) as site_key.
				
	{link} this is a social bookmark tag that will be replaced with the user's web page URL automatically.
	
	{title} this is  a social bookmark tag that will be replaced with the user's web page title automatically.

Once you have finished editing the sites_template.xml, rename it to sites_XX.xml where XX shoud be the ISO 
country code for the language that you are working on.



Note 1: In the url, you need to change any '&' characters to '&amp;' (without the quotes) otherwise your file 
		would not be a valid XML file.

Note 2: Make sure that you do not delete the <social></social> tags.

Note 3: Once you have finished your button, you can sately remove the images/template.png and sites_template.xml files
		before you make a zip file and you distribute your language pack on the web.

Note 4: Have a look in the language pack that is included with Social Bookmarks to get a better idea!

