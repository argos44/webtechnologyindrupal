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
