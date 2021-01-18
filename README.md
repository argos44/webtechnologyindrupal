# webtechnologyindrupal
how drupal's twig templates improve web security

Almost half or more of the world's web pages are based on Drupal. But it may be more..... why?

Drupal templates are basically CSS configurations.

Read here, what is CSS:

https://developer.mozilla.org/en-US/docs/Web/CSS

So, Drupal works in a way, that it is graphical, meaning, you don't have to program a line to create a stunning webpage.

From the graphical layout you created, adding pictures, texts, newsletters, stories, interactive elements, etc... (payment is NOT drupal, that is usually safe).

from those elements, the DRUPAL twig engine generates a PHP code. That is called a server side script, because it is not visible from the not, it is not included in search engine hits.

see here:

https://www.drupal.org/docs/theming-drupal/twig-in-drupal/debugging-compiled-twig-templates


If you click on the webpage nameadress, the TWIG engine generates a HTML code from the PHP (server-side) code, and displays it to you. This can happen anytime you click on the page, or while you're reading it, not doing any interaction, or never.

This is dependent on TWIG parameter coding, which is basically a security paramater, which tells the engine whether the template used is used by a trusted member, or it is someone else.

This is written here:

https://dev.acquia.com/blog/debugging-twig-templates-in-drupal-8-with-phpstorm-and-xdebug/25/08/2016/16586


************************************


Soo.... it is actually quite easy....

https://imgur.com/a/2ITO8EC

Frontpage is sitename/node

  a node is just a content management structure, it is a content, that has different aspectual values (just being smart), which just means that different   aspects of the content are included in the concept of node, like comments for an image, image resolution, URL aliases, etc.

change that to the URL that loads when you enter your homepage.

Then change that to /home, for example.

Frontpage is from where you have to remove all unnecessary things like site branding logos, breadcrumbs, etc etc. You can disable those things under blocks menu in admin/structure

Change theme to Claro. Use Php 7.0 you'll see why.

If you removed everything, then type sitename/admin to enter admin.

Then, as you can see on the images, you can add your own custom .css files. It is called a wrapper-class. It is under views menu of the Frontpage.

Adding relationships is useful when trying to add extensions of the responsive image class, and you want to link different aspects of nodes. I'm not sure about that, though.

For instance, if you would like to display an image, add the image extension, create a new content type, and if the extension image is added, you can add an image field to that content type.

Yes, relationships are linking fields from different things, and fields are aspects of nodes, that is, they are aspects of content types (so alltogether they form an entity called node)

have fun! mess around, take your time, see this, see that, you never know how you managed to make it look  ok :)))





