.. sectionauthor:: Artem Svetlov <artem.svetlov@nextgis.ru>

.. _ngsimplecollector_intro:


Introduction
=============

.. _ngsimplecollector_purpose:

**Simple Collector** is an Android application that uses nextgis.com Web GIS for field data collection. Simple Collector provides simpler workflow than Formbuilder + NextGIS Mobile at expense of flexibility. Simple Collector is super easy to use for surveyors and requires just a little bit a set up.


.. figure:: _static/ng_simplecollector_mobile_1_ru.png
   :name: nng_simplecollector_mobile_1_ru
   :align: center
   :height: 10cm
  
   Mobile app window.

Features
--------
* Mobile app is freely available on Google Play.
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

.. figure:: _static/ng_simplecollector_mobile_1_ru.png
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

.. figure:: _static/ng_simplecollector_desktop_1_ru.png
   :name: ng_simplecollector_desktop_1_ru
   :align: center
   :height: 10cm
  
   Collected data appear in desktop software NextGIS QGIS




