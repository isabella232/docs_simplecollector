.. sectionauthor:: Artem Svetlov <artem.svetlov@nextgis.ru>

.. _ngsimplecollector_intro:


Введение
========

.. _ngsimplecollector_purpose:

**Простые учёты** это приложение для Android использующее Веб ГИС для сбора данных в поле. Простые учёты является альтернативой более сложным и универсальной связке Formbuilder + NextGIS Mobile. Приложение очень легко настраить и максимально просто в использовании для сборщиков.


.. figure:: _static/ng_simplecollector_mobile_1_ru.png
   :name: nng_simplecollector_mobile_1_ru
   :align: center
   :height: 10cm
  
   Общий вид окна программы

Как это работает
----------------
* Мобильное приложение свободно доступно на `Google Play <https://play.google.com/store/apps/details?id=com.nextgis.simple_collector>`.
* Настройка проекта по сбору данных делается через Веб браузер в интерфейсе Веб ГИС.
* Сборщику нужно только установить приложение, ввести имя Веб ГИС, логин и пароль.
* Приложение автоматически синхронизирует данные с Веб ГИС. Данные не потеряются даже если пропадет интернет или отключится телефон/планшет.  Как только связь появится, синхронизация продолжится.
* Форма данных намерено максимально упрощен: точки с координатами, имя сборщика, тип объекта и несколько дополнительных полей. Данные легко загрузить и обработать в ГИС.

Установка для администратора
============================

1. Get access to Simple Collector for you nextgis.com account.
2. Download NextGIS Simple Collector from Google Play.
3. Start NextGIS Simple Collector, provide Web GIS name, login and password. Mobile application will initialize data structure in you Web GIS.

Создание проекта по сбору данных
================================

5. Open Web GIS in your Web browser. A new group “ Simple collector, data” will appear in the root folder.
6. Add surveyors. Go to “People” lookup table → Update, add field crew.

.. figure:: _static/ng_simplecollector_add_surveyors_1_ru.png
   :name: ng_simplecollector_add_surveyors_1_ru
   :align: center
   :height: 10cm
  
   Добавление сборщиков


7. Add surveyed “objects” list. Each object will be shown as a button for surveyor. Go to “objects’ lookup table → Update, and add record with browser. 

.. figure:: _static/ng_simplecollector_objects_1_ru.png
   :name: ng_simplecollector_objects_1_ru
   :align: center
   :height: 10cm
  
   Добавление собираемых объектов
   

8. At your mobile device, click “Synchronize”. Your simple form will appear.

.. figure:: _static/ng_simplecollector_mobile_1_ru.png
   :name: nng_simplecollector_mobile_retry_ru
   :align: center
   :height: 10cm
  
   Your form in mobile app window.
   
9. Share

Ask surveyors to install Simple Collector. Let them know Web GIS name, login and password. Create of multiple users in WEB Gis avaible at high tarifs. On simple tariff you can provide ownself login and password, but any surveyor can delete any data using web browser.

Начало работы для сборщика
==========================

1. Download NextGIS Simple collector on `Google Play <https://play.google.com/store/apps/details?id=com.nextgis.simple_collector>`.
2. Fill Web GIS name, login and password, provided by administrator
3. You will see a list of surveyors. Select one.
4. You can hit “Synchronize” to see the latest changes to the structure.
5. Go outside, hit “Start track” and then use buttons on the form to collect data.

После окончания сбора
=====================

Data will added as a Web GIS vector layer. You can download in as a GeoJSON or CSV in EPSG:3857 coordinate system.

Easier workflow: start desktop software NextGIS QGIS, connect to your Web GIS using NextGIS Connect plugin, and download layer right in  your GIS.

.. figure:: _static/ng_simplecollector_desktop_1_ru.png
   :name: ng_simplecollector_desktop_1_ru
   :align: center
   :height: 10cm
  
   Собранные данные в NextGIS QGIS




