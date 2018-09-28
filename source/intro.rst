.. sectionauthor:: Artem Svetlov <artem.svetlov@nextgis.ru>

.. _ngsimplecollector_intro:


Introduction
=============

.. _ngsimplecollector_purpose:

**Simple Collector** is an Android application that uses nextgis.com Web GIS for field data collection. Simple Collector provides simpler workflow than Formbuilder + NextGIS Mobile at expense of flexibility. Simple Collector is super easy to use for surveyors and requires just a little bit a set up.


.. figure:: _static/ng_simplecollector_mobile_1_ru.png
   :name: nng_simplecollector_mobile_1_ru
   :align: center
   :scale: 30%
  
   Mobile app window.

Features
--------
* Mobile app is freely available on `Google Play <https://play.google.com/store/apps/details?id=com.nextgis.simple_collector>`_.
* Configuration of data structure can be done via Web browser at your nextgis.com instance.
* Surveyor just needs to install and app, fill Web GIS name, login and password.
* Mobile app automatically syncs data with your Web GIS. In case there is no internet access, device reboot, or pause in surveying - data will not be lost. It will be sent to the server when connectivity is restored.
* Data structure is as simple as possible: only points with coordinates, surveyor id, type of object and some additional fields. No long hard to analyze sets of fields. Only machine-readable data that can be processed using GIS methods.

Installation
============

1. Get access to Simple Collector for you nextgis.com account.
2. Download NextGIS Simple Collector from Google Play.
3. Start NextGIS Simple Collector, provide Web GIS name, login and password. Mobile application will initialize data structure in you Web GIS.

Create data structure
=====================

5. Open Web GIS in your Web browser. A new group “ Simple collector, data” will appear in the root folder.
6. Add surveyors. Go to “People” lookup table → Update, add field crew.

.. figure:: _static/ng_simplecollector_add_surveyors_1_ru.png
   :name: ng_simplecollector_add_surveyors_1_ru
   :align: center
   :height: 10cm
  
   Add surveyors.


7. Add surveyed “objects” list. Each object will be shown as a button for surveyor. Go to “objects’ lookup table → Update, and add record with browser. 

.. figure:: _static/ng_simplecollector_objects_1_ru.png
   :name: ng_simplecollector_objects_1_ru
   :align: center
   :height: 10cm
  
   Add objects of survey.
   

8. At your mobile device, click “Synchronize”. Your simple form will appear.

.. figure:: _static/ng_simplecollector_mobile_1_ru.png
   :name: nng_simplecollector_mobile_retry_ru
   :align: center
   :scale: 30%
  
   Your form in mobile app window.
   
9. Share

Ask surveyors to install Simple Collector. Let them know Web GIS name, login and password. Create of multiple users in WEB Gis avaible at high tarifs. On simple tariff you can provide ownself login and password, but any surveyor can delete any data using web browser.

Manual for surveyors
====================

1. Download NextGIS Simple collector on `Google Play <https://play.google.com/store/apps/details?id=com.nextgis.simple_collector>`_.
2. Fill Web GIS name, login and password, provided by administrator
3. You will see a list of surveyors. Select one.
4. You can hit “Synchronize” to see the latest changes to the structure.
5. Go outside, hit “Start track” and then use buttons on the form to collect data.

After data collection
=====================

Data will added as a Web GIS vector layer. You can download in as a GeoJSON or CSV in EPSG:3857 coordinate system.

Easier workflow: start desktop software NextGIS QGIS, connect to your Web GIS using NextGIS Connect plugin, and download layer right in  your GIS.

.. figure:: _static/ng_simplecollector_desktop_1_ru.png
   :name: ng_simplecollector_desktop_1_ru
   :align: center
   :height: 10cm
  
   Collected data appear in desktop software NextGIS QGIS




