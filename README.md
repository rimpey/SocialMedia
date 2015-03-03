![alt text](http://docs.rhondaimpey.com/img/socialmedia.jpg "Social Media")

SocialMedia
===========

Social Media Icons for; LinkedIn, Github, YouTube, Twitter, Facebook, Pinterest, Instagram

Using a site called addthis.com to generate social plugins.
 1. create an account where analytic statistics will be available
 2. go to 'Follow Buttons' hovering over the 'Get the code' button to access
 3. stipulate follow buttons for a website with horizontal large menu layout
 4. for each media site required fill in the username each will be auto included in the 'Grab It' code
 
'''
 http://facebook.com/rimpey
 http://twitter.com/rhondaimpey
 http://linkedin.com/in/rhondaimpey
 http://youtube.com/user/RhondaImpey
 http://pinterest.com/rimpey
 http://instagram.com/rhondaimpey
 '''

copy the code provided and past directly inbetween the body and /body tags
 
The link to GitHub needed to be added separately however the layout and spans came for free with the assumed and
correct line of code (even though not listed on the media site):
    
    '''
    <a class="addthis_button_linkedin_follow" addthis:userid="rhondaimpey"></a>
    '''
    
The icons provided can be replaced and styled in accordance with the website styling theme. I chose to use some free
greyscale icons that I discovered on-line from: 

     '''
     http://tomswebspace.com/round-social-media-icons/
     ''' 
     
and created a singular image of 6 32x32 pixel images on top of each other; dimensions 32pixels wide 
and 224pixes high as a single image is more desirable for download than many small images.

The background position was used to position horizontal (xpos) and vertical (ypos) placement for each media icon
in turn decreasing the ypos by the height of the above icon -32px each time, place important to override styling 
according to the attached addthis style sheet, otherwise the default style media icons will be used. 

Classes that needed to be overridden in the addthis style sheet for icon placement could only be viewed in the 'inspect
element' developer tools after the minified style sheet had been applied. Hence the classes:


- .at15t_linkedin,.at15t_github,.at15t_youtube,.at15t_twitter,.at15t_facebook,.at15t_pinterest,.at15t_instagram

could have the icon placement overridden.

Finally a click event on the GitHub icon needed to be created as this was not supplied as part of the addthis social
media plugin, so this is added using the .addthig_button_github_follow class and directs it's href to the http address
with user name.

    
 ===================================================================================================================
 03/03/2015
 
 Update README


AddThis.com changed class names which broke my code

In order to retain my specially designed grey icons I needed to change the class names to reflect those changed by AddThis.com otherwise the ugly default icons were displayed on my website, not in keeping with my design.

Class name changes are as follows:

 .at15nc is now => .at4-icon
 .at15t_linkedin is now => .aticon-linkedin

I've changed my style sheets accordingly.
 
