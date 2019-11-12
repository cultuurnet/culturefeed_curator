Culturefeed Curatoren
===========

This module allows you to make requests to the Curator API to be able to retrieve external articles for an UDB item.
The module will automatically preprocess the culturefeed events with the articles.

## Configuration
The module can be configured at Settings > Culturefeed > Culturefeed Curatoren API (admin/config/culturefeed/curator)
It is default configured to use the live api.

## Using the module
The module handles the preprocessing for culturefeed event. The templates will receive an array called 'external_article_links'. The array contains all the links.
```
<ul>
<?php foreach ($external_article_links as $external_article_link): ?>
  <li><?php print $external_article_link; ?></li>
<?php endforeach; ?>
</ul>
```
 
