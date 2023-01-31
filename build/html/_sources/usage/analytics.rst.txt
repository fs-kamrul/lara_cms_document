
Analytics
#########

Integrate with Google Analytics

.. image:: /images/analytics.png

Getting credentials
===================

* Video tutorial:

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>

* Go to https://console.developers.google.com/apis/dashboard and create a new project

.. image:: /images/analytics1.png

.. image:: /images/analytics2.png

.. image:: /images/analytics3.png

* Select your project and click on **"ENABLE APIS AND SERVICES"**:

.. image:: /images/analytics4.png

* Enable API:

.. image:: /images/analytics5.png

.. image:: /images/analytics6.png

.. image:: /images/analytics7.png

* Generate service account key:

.. image:: /images/analytics8.png

.. image:: /images/analytics9.png

.. image:: /images/analytics10.png

.. image:: /images/analytics11.png

.. image:: /images/analytics12.png

.. image:: /images/analytics13.png

.. image:: /images/analytics14.png

.. image:: /images/analytics15.png

.. image:: /images/analytics16.png

.. image:: /images/analytics17.png

* Open JSON file and copy its content, then go to Dashboard -> Settings (/systemsettings/settings) and update field "Service Account Credentials" in Analytics plugin settings by the content from JSON file:

.. image:: /images/analytics29.png

It will look like this:

Setting Google Analytic
=======================

* Go to Google Analytics account: https://analytics.google.com/analytics/web/. Click on "Admin" => "View Settings" and copy "View ID" number, then go to /systemsettings/settings and tab "Google Analytics" and paste to field View ID.

.. note::
   Note: Change in Google Analytics 4 property.

.. image:: /images/analytics18.png

.. image:: /images/analytics19.png

.. image:: /images/analytics20.png

.. image:: /images/analytics21.png

When creating a new property, you need to check the "Create a Universal Analytics Property" checkbox.

.. image:: /images/analytics22.png

.. image:: /images/analytics23.png

Then you will have view settings tab and View ID.

.. image:: /images/analytics24.png

Then you will have view settings tab and Tracking ID.

.. image:: /images/analytics25.png

* Open JSON credentials file and copy client email. Then click on "User management" and add that email to list account. Just need view only permission.

.. image:: /images/analytics27.png

.. image:: /images/analytics28.png

Setup timezone and clear cache
==============================

* Go to Dashboard -> Cache management and clear your site cache.

.. image:: /images/cache_commands.png

.. note::
   Analytics data in Admin dashboard is displayed daily data, so it will reset chart every day. It is displaying data from API, not realtime analytics so please wait until your site has data from API.

Give your comment here if you got any problem.

Good luck!