Modified Lightbox2 v1.1

Modified Code for HTML5 Compliance/Validation By David Gladwin - http://www.gladwinput.com

Original Code By Lokesh Dhakar - http://www.lokeshdhakar.com

This script itself (Originally the Lightbox2 script by Lokesh Dhakar) was fantastic, however in HTML5 the rel= attribute did not validate. This was a problem for university work. I've made some small modifications to the script to make up for this drawback. Some mild changes to implementation as well - however otherwise very similar. I've also removed some depricated code so it will now work with jquery 1.9.1. Thanks to Lokesh for original script.

Licensed under the Creative Commons Attribution 2.5 License - http://creativecommons.org/licenses/by/2.5/
- free for use in both personal and commercial projects
- attribution requires leaving author name, author link, and the license info intact.

HOW TO USE:

First - Add the img, css and js files. And check that you have changed the /img/ reference in both css and js files to point to the correct folder on your website

Second -  make sure you have jquery added into your page in <head> like this (I use googleapis):
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js" type="text/javascript"></script>

(You can use 1.9.1 - as there was a fault when using 1.9.1 with the original script where the images didn't appear withhe original script.)

Third - Call the js file in through your header like this:
<script src="js/lightbox.js"></script>

Fourth - Wherever you want an image to show up, use 'class="lightbox"' in the <a> tag.
Examples:

<a class="lightbox" href="img/WestLulworth.jpg" title="my caption"><img src="/img/WestLulworth.jpg" alt="West Lulworth"></a>

<a class="lightbox bus" href="img/WestLulworth.jpg" title="my caption"><img src="/img/EastLulworth.jpg" alt="West Lulworth"></a>

<a class="lightbox bus" href="img/WestLulworth.jpg" title="my caption"><img src="/img/LulworthCove.jpg" alt="West Lulworth"></a>

Note that your images will auto group according to the link class. So if you have two tags like class="lightbox bus" for example (though it can be anything, doesnt have to be 'bus'), they will group up. If you simply have 10 "lightbox" images without group names, they will ALL group up. So in the above example you will have a group of 2, and 1 image just lightboxing by itself.

Not all have "title" attributes, which give a caption, you don't actually have to supply this attribute, if you don't, there won't be a caption.

That is all. Thank you very much for downloading this, thank you very much to Lokesh Dhakar for coding the original lightbox2 (it's over 5 years old I believe, and very popular!) I hope my modifications to make it validate with HTML5 are useful to you :) Please leave the credit header in the js so that Lokesh's work is credited if you are going to use it, as per the original license.

Incidentally, should probably have used data- as html5 gives that option, it would also have meant that "lightbox" by itself wouldn't cause a bunch of images to group up. But feh, this does the trick and depricates nicely to IE.