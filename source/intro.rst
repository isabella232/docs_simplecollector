.. sectionauthor:: Artem Svetlov <artem.svetlov@nextgis.ru>

.. _ngsimplecollector_intro:


Introduction
=============

.. _ngsimplecollector_purpose:

**Simple Collector** - complex of Android application and nextgis.com settings for field data collections. It provider more simpler workflow than Formbuilder + Nextgis Mobile solution.


.. figure:: _static/nng_simplecollector_mobile_1_ru.png
   :name: nng_simplecollector_mobile_1_ru
   :align: center
   :height: 10cm
  
   Mobile app window.

Installation
==============

1. Get access to Simple Collector for you nextgis.com account.
2. Download NextGIS Simple Collector from Google Play.
3. Start NextGIS Simple Collector on Android, provide nextgis.com account, and your WEB GIS login and password. Mobile application will create ownself data structure in you WEB GIS.

Create data structure
===========================

5. Open WEB GIS in desktop browser. A new group “Простые учёты, сбор данных” will appear.


   
   
6. Add field editors. Go to “Учётчики” lookup table → Update, add users using web browser.


.. figure:: _static/ng_simplecollector_add_surveyors_1_ru.png
   :name: ng_simplecollector_add_surveyors_1_ru
   :align: center
   :height: 10cm
  
   Add surveyours.


7. Add “objects of survey” - it shown as button for surveyor. Go to “objects’ lookup table → Update, and add record with browser. 

.. figure:: _static/ng_simplecollector_objects_1_ru.png
   :name: ng_simplecollector_objects_1_ru
   :align: center
   :height: 10cm
  
   Add objects of survey.
   

8. At your mobile device, click “Sinchronize”. Your simple form will appear.

.. figure:: _static/nng_simplecollector_mobile_1_ru.png
   :name: nng_simplecollector_mobile_retry_ru
   :align: center
   :height: 10cm
  
   Your form in mobile app window.
   

You should provide an URL, Login and Password for surveyors. Create of multiple users in WEB Gis avaible at high tarifs. On simple tariff you can provide ownself login and password, but any surveyor can delete any data using web browser.

Manual for surveyors
============================

1. Download NextGIS Simple collector in Google Play
2. Fill URL, login and password, witch administrator you provide
3. You will get a list of user. Select own.
4. Since this time you can call “Synchronize” every time, when administrator made a changes in structure.
5. Go outside, push “Start” and then buttons in form

After data collection
=============================

Data will added in WEB Gis vector layer. You can download in as file in web interface, it will be GeoJSON file with nodes in EPSG:3857 coordinate system, or as CSV and compute it in other software.

More easy workflow: start desktop software NextGIS QGIS, connect to your WEB Gis using NextGIS Connect module, and download layer.


