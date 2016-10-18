Connections
===========

.. contents::
   :backlinks: top
   :local:
   
Exterior Cables & Hoses
-----------------------

.. warning::
   The bulkhead connectors are tightened against mounting surfaces. MOLYKOTE 44 MEDIUM grease is applied to all male pins before mating.

.. note::
   - SubConn `Power`_ Series information.
   - SubConn `Micro`_ Circular Series information.

You can download :download:`this cabling diagram </_static/CablingDiagram.pdf>` or :download:`this block diagram </_static/FunctionalBlockDiagram(8).pdf>`.


Main Housing I/O Panel -- Port
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. image:: /_static/io_panel_port.png

.. note::
   All SubConns have strain reliefs with the exception of bottom port surge.

+---------------------------+-----------------+--------+----------------+
| Connection                | Series          | # Pins | Amps/Connector |
+===========================+=================+========+================+
| Acoustics Housing         | Micro Circular  |  4     |  20            |
+---------------------------+-----------------+--------+----------------+
| Kill Switch               | Micro Circular  |  4     |  20            |
+---------------------------+-----------------+--------+----------------+
| Battery Housing -- Port   | Micro Circular  |  4     |  20            |
+---------------------------+-----------------+--------+----------------+
| Battery Housing -- Port   | Power           |  4     |  50            |
+---------------------------+-----------------+--------+----------------+
| Pneumatics Housing        | Micro Circular  |  4     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Upper Surge   | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Lower Surge   | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Forward Heave | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- After Heave   | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Forward Sway  | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+

Main Housing I/O Panel -- Starboard
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. image:: /_static/io_panel_stbd.png

.. note::
   All SubConns have strain reliefs with the exception of bottom starboard surge.

+---------------------------+-----------------+--------+----------------+
| Connection                | Series          | # Pins | Amps/Connector |
+===========================+=================+========+================+
| Pneumatics Housing        | Micro Circular  |  4     |  20            |
+---------------------------+-----------------+--------+----------------+
| Battery Housing -- Stbd   | Micro Circular  |  4     |  20            |
+---------------------------+-----------------+--------+----------------+
| Battery Housing -- Stbd   | Power           |  4     |  50            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Upper Surge   | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Lower Surge   | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Forward Heave | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- After Heave   | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Thruster -- Aft Sway      | Micro Circular  |  3     |  20            |
+---------------------------+-----------------+--------+----------------+
| Tether                    | Ethernet        |  8     |                |
+---------------------------+-----------------+--------+----------------+

Pneumatics Housing (Hoses)
~~~~~~~~~~~~~~~~~~~~~~~~~~

+---------------------------+----------+----------+
| Connection                | Color    | Diameter |
+===========================+==========+==========+
| Supply                    |          |          |
+---------------------------+----------+----------+
| Manipulator -- Port       |          |          |
+---------------------------+----------+----------+
| Manipulator -- Stbd       |          |          |
+---------------------------+----------+----------+
| Marker Dropper -- Port    |          |          |
+---------------------------+----------+----------+
| Marker Dropper -- Stbd    |          |          |
+---------------------------+----------+----------+
| Torpedo Launcher -- Port  |          |          |
+---------------------------+----------+----------+
| Torpedo Launcher -- Stbd  |          |          |
+---------------------------+----------+----------+


SubConn Pinouts
~~~~~~~~~~~~~~~

**Power**

=== ===== ======
Pin Color Signal
=== ===== ======
1   White B+
2   White B-
3   White NC
4   White NC
=== ===== ======


.. _Power: http://www.macartney.com/what-we-offer/systems-and-products/connectivity/subconn/subconn-power-series/subconn-power-battery-2-3-and-4-contacts/
.. _Micro: http://www.macartney.com/what-we-offer/systems-and-products/connectivity/subconn/subconn-micro-circular-series/subconn-micro-circular-2-3-4-5-6-and-8-contacts-and-g2-2-3-and-4-contacts/
