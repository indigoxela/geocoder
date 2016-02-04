Geocoder
========

                            (
     (  (    (               )\ )  (  (
     )\))(  ))\ (    (  (   (()/( ))\ )(
    ((_))\ /((_))\   )\ )\   ((_))((_|()\
     (()(_|_)) ((_) ((_|(_)  _| (_))  ((_)
    / _` |/ -_) _ \/ _/ _ \/ _` / -_)| '_|
    \__, |\___\___/\__\___/\__,_\___||_|
    |___/

#### Contents of this File

 * About Geocoder
 * Install
 * Configure
 * Credits

About Geocoder
--------------

Geocoder is a Drupal 7 module that will extract geographical data (geocode) 
from just about anything you throw at it such as addresses, GPX files, Geotags 
from EXIF data in photos, and KML files.

A convenient way to allow users to enter an address and have it automatically 
geocoded is to use it in combination with the Addressfield 
(http://drupal.org/project/addressfield) and Geofield 
(http://drupal.org/project/geofield) modules.

Geocoder uses the external geocoding services from Google, Yahoo and Yandex.

Here you find great documentation on Geocoder: http://drupal.org/node/1355780

Install
-------

- Install this module using the official Backdrop CMS instructions at 
  https://backdropcms.org/guide/modules
- Install required module geoPHP
- Install optional modules Addressfield and Geofield

Configure
---------

Assign the necessary permissions at /admin/people/permissions#module-geocoder

If you have enabled the modules Addressfield and Geofield you can start using Geocoder in a content type, e.g., an event.

Add a new address field by going to /admin/structure/types, choosing the 
desired content type and opening the "Manage fields" tab. Add a "Postal 
address" field and configure the field. Add a geofield and select "Geocode 
from another field" as widget. In the settings for the geofield you can now 
choose the source field to geocode from. You can also choose which geocoding 
service (Google et cetera) to use and configure these services.

Now you have a place where Geocoder can store its result (geofield) and the 
input to the geocode operation (addressfield). You can then use 
OpenLayers to map the geofields.

Note: you can use Geocoder in any entity such as a user, a taxonomy term or 
a comment.

Current Maintainers
-------------------

- Wes Jones (https://github.com/earthday47)
- gifad (https://github.com/gifad)

Credits
-------

- Ported to Backdrop CMS by gifad (https://github.com/gifad)
- Originally written for Drupal by: cspiker, phayes, henryblyth, jeff h, 
  Les Lim, mikeytown2, fago, patrickavella & michaelfavia
