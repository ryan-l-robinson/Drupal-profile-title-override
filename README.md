## Overview

This provides a demonstration of configuration as well as custom code to override the title of a staff profile created with the Drupal profile module, so that the title will appear as the profile's First Name and Last Name instead of as "Staff Profile #1."

The entire Drupal configuration is provided, to [work with GitPod](https://github.com/ryan-l-robinson/Drupal-GitPod) for quick demonstration purposes. 

## Custom Module

The page's title tag (that appears in the browser's header) is accomplished with custom code. It can be seen in /web/modules/custom/profile_title.

## View

The page's title that appears as a header 1 on the page is accomplished with a view block added to the profile's layout. This can be seen in multiple configuration files including:

- views.view.profile (creating the view)
- block.block.views_block__profile_block_1 (adding the custom page title block)
- block.block.olivero_page_title (removing the default page title)
- core.entity_view_display.profile.staff_profile.default (removes the first name and last name from displaying again, since it is already in the title view)