## Layout Paragraphs Starterkit Default Content


This Custom Default Content module relies and depends upon the Drupal 8 [Default Content module](https://www.drupal.org/project/default_content)

### Module usage:

Example for exporting Content (and related) entities, process all the followings
from the drupal app root (/web);

    drush dcer node --folder=modules/custom/custom_default_content/content -y
    drush dcer paragraph --folder=modules/custom/custom_default_content/content -y
    drush dcer media --folder=modules/custom/custom_default_content/content -y
    drush dcer file --folder=modules/custom/custom_default_content/content -y


