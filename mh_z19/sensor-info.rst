mh_z19
=============

MH-Z19B 
---------

Infrared Carbon Dioxide Monitor Sensor CO2 Detection Sensor Module (CO2 二氧化碳感測器)

- `Official User Manual <https://www.winsen-sensor.com/d/files/infrared-gas-sensor/mh-z19b-co2-ver1_0.pdf>`_

- `Arduino Library | mh-z19 <https://github.com/WifWaf/MH-Z19/blob/master/README.md>`_

- `Raspberry Pi Sensor Libraries | mh-z19 <https://pypi.org/project/mh-z19/>`_

|

.. raw:: html

  <img src="https://www.winsen-sensor.com/d/propic/MH-Z19B.jpg" alt="" width="300" height="300">

|

Sensor Spec

.. code::

  Technical Parameters:
  Target Gas: CO2
  Measuring Range: 0-5000 ppm
  Accuracy: ±(50ppm + 5% readings)
  Working Voltage: 3.6 to 5.5 V DC
  Average Current: < 18 mA
  Interface Level: 3.3 V
  Measuring range: 0 to 0.5% Vol Optional
  Output Signal: UART; PWM
  Preheat Time: 3 min
  Response Time: T90 < 60s
  Working Temperature: 0 to 50℃
  Working Humidity: 0 to 95% RH (No condensation)
  Dimension:33 mm x 20 mm x 9 mm (L*W*H)
  Weight: 21 g


|


Cabling (佈線)
++++++++++++++++

|

Connect RPi & mh-z19 as:

- 5V on RPi and Vin on mh-z19
- GND(0v) on RPi and GND on mh-z19
- TxD and RxD are connected to cross between RPi and mh-z18

|

.. raw:: html

  <img src="https://warehouse-camo.ingress.cmh1.psfhosted.org/5e69358ea376cf9c8460b74610e3cd2ca2f487f9/68747470733a2f2f63616d6f2e67697468756275736572636f6e74656e742e636f6d2f336364346331623438326561393032623765363664636131336434323630313933633833316136332f3638373437343730373333613266326636333631366436663265373136393639373436313735373336353732363336663665373436353665373432653633366636643266333133313332363136343335363636353334333136333338333236313331333633363337333136343332333833383332333033373330333333383334333133303339363333383338333633303633363332663336333833373334333733343337333033373333333336313332363633323636333733313336333933363339333733343336333133323634333633393336363433363331333633373336333533323634333733333337333433363636333733323336333533323635333733333333333333323635333633313336363433363331333736313336363633363635333633313337333733373333333236353336333333363636333636343332363633333330333236363333333433333336333333353333333433333334333236363333333033333338333333323333333833333333333333303333333133333334333236343333333633333338333633343333333233323634333633333333333333363334333633353332363433333331333333363333333433333334333236343333333733363333333333383336333433333339333633323333333733363332333333363333333233363336333633343332363533363631333733303336333533363337" alt="" width="500" height="500">


|

Installation

.. code:: py

  pip install mh_z19



Use as python script.

.. code:: py

  pi@raspberrypi:~/mh-z19/pypi $ sudo python -m mh_z19
  {'co2': 500}


Import module and call read()

.. code:: py

  pi@raspberrypi:~/mh-z19/pypi $ sudo python
  Python 2.7.13 (default, Nov 24 2017, 17:33:09) 
  [GCC 6.3.0 20170516] on linux2
  Type "help", "copyright", "credits" or "license" for more information.
  >>> import mh_z19
  >>> mh_z19.read()
  {'co2': 477}
  >>> 



readall()

.. code:: py

  >>> import mh_z19
  >>> mh_z19.read_all()
  {'SS': 232, 'UhUl': 10738, 'TT': 61, 'co2': 734, 'temperature': 21}
  >>> 

|

Use specific serial device

.. code:: py

  sudo python -m mh_z19 --serial_device /dev/ttyUSB0


|

Reference
-----------

- `mh-z19 | PyPI <https://pypi.org/project/mh-z19/>`_



|
