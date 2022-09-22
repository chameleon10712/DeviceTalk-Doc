DeviceTalk Documentation
===========================

- `DeviceTalk User Manual | HackMD <https://hackmd.io/@Eric-Pwg/SJWlETzj5/https%3A%2F%2Fhackmd.io%2F%40Eric-Pwg%2FB1W18mViq>`_
- `DeviceTalk Source Code | GitHub <https://github.com/IoTtalk/DeviceTalk/tree/sersor-journal>`_
- `IoTtalk - DeviceTalk Library file | GitHub <https://github.com/IoTtalk/DeviceTalk-Library-file>`_

  - Eric
  - `DeviceTalk Libray File 檔案結構 | HackMD <https://hackmd.io/@Eric-Pwg/SJWlETzj5/https%3A%2F%2Fhackmd.io%2F%40Eric-Pwg%2FB15oVAaO9>`_

- `DeviceTalk Demo Video | HackMD <https://hackmd.io/@Eric-Pwg/SJWlETzj5/https%3A%2F%2Fhackmd.io%2F%40Eric-Pwg%2FHkRRh7Vs9>`_

|

Sensors
---------

.. list-table:: List
   :widths: 50 50 50 50
   :header-rows: 1

   * - Type
     - 
     - Sensor
     - 
   * - Temperature and Humidity Sensor
     - 溫濕度感測器
     - DHT11
     - DHT22
   * - Infrared carbon dioxide (CO2) sensor
     - CO2 感測器
     - MH-Z19
     - T6603
   * - I2C Oxygen Sensor
     - 空氣品質感應器
     - SEN0322
     - 
     
|


Demo
------------

Plantbox

- dht11
- mhz_19
- sen0322

|

DeviceTalk
-------------

- device-talk

  - devicetalk
  
    - views.py
    
      - MainPageView
    
  - xtalk_account
 
    - views.py
    
      - AuthRedirectionView
      - LogoutView
      - AuthCallbackView
   
  - file_handle

    - views.py

      - FileView
      - UploadSetupView

  - my_admin
  
    - views.py
    
      - LanguageView
      - BasicFileView
      - IndexView

  - api
  
    - views.py
    
      - LibraryManagerView
      - ListFunctionManagerView
      - NewFunctionManagerView
      - SingleFunctionManagerView
      - DeviceManagerView
      
    - models.py
    
      - `DeviceTalk 資料庫說明 | HackMD  <https://hackmd.io/@Eric-Pwg/HJSaW_2Oc#DeviceTalk-%E8%B3%87%E6%96%99%E5%BA%AB%E8%AA%AA%E6%98%8E>`_

|

Django Data Flow Diagram
--------------------------

.. image:: https://i.stack.imgur.com/r91Zn.png

|

DeviceTalk Apps
------------------

.. raw:: html

  <img src="https://i.imgur.com/dkW2FVA.png" alt="" width="800" height="">


|

DB Schema
------------

.. image:: https://i.imgur.com/u7SKO36.png

|

Docker Architecture
---------------------

.. image:: https://docs.docker.com/engine/images/architecture.svg

