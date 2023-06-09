## Layout Paragraphs Starterkit
for Drupal 10
___
### How to install and setup with test/start content.

Clone this repository in your local env/machine

    git clone https://github.com/itamair/drupal_layout_paragraphs_starterkit.git

and move into the cloned repository folder:

    cd drupal_layout_paragraphs_starterkit

To run this Drupal instance locally it is advised to use DDEV.

[DDEV Installation](https://ddev.readthedocs.io/en/latest/users/install/)

Note: Whatever system you’re on, you’ll first need to Install Docker or Colima,


From your project/root folder install the project dependencies:

    composer install


Build the containers and set up the Drupal project with the following command:

    ddev start

Get into the web container via ssh, through the following command:

    ddev ssh

and finally, import the test/start content with the following content
(still from the web container):

    drush sql-cli<db_dumps/db_start.sql

Check the drush import of the Drupal configurations
(still from the web container):

    drush cim -y

(there shouldn't any change to import, or only language.negotiation Update).

then you will be All Set!

The Layout Paragraphs Starterkit Drupal website should be reachable at the following link:

    https://drupal-layout-paragraphs-starterkit.ddev.site

You should Login with Administrator Credentials:

      username: admin
      password: admin

and then test Layout Paragraphs functionalities directly from the Home Page Content.
