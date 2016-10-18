Main Housing
============

.. contents::
   :backlinks: top
   :local:


Motherboard
-----------

Jumper Configuration
~~~~~~~~~~~~~~~~~~~~

.. image:: ../_static/motherboard.jpg

+----------------------------------------------+------------------+-------------+--------------------------------------------+
| Name                                         | Setting for AUV  | Pins Jumped | Notes                                      |
+----------------------------------------------+------------------+-------------+--------------------------------------------+
| Clear CMOS (JCMOS1)                          | Normal (Default) | 1 - 2       | Use to reset if board overheats and locks. |
+----------------------------------------------+------------------+-------------+--------------------------------------------+
| AT/ATX Power Mode Select (PSON1)             | AT Mode          | 1 - 2       | Boot on power (bypass button)              |
+----------------------------------------------+------------------+-------------+--------------------------------------------+
| Chassis Intrusion Connector (JCASE1)         | Default          | 1 - 2       | Leave jumper on connector                  |
+----------------------------------------------+------------------+-------------+--------------------------------------------+
| COM1/COM2 RI/+5V/+12V Mode Select (JCOMPWR1) | 12V              | 3 - 4       |                                            |
+----------------------------------------------+------------------+-------------+--------------------------------------------+
| COM3/COM4 RI/+5V/+12V Mode Select(JCOMPWR2)  | 12V              | 3 - 4       |                                            |
+----------------------------------------------+------------------+-------------+--------------------------------------------+
| M-SATA/mini PCIe Select (JMSATASW1)          | MSATA            | 1 - 2       |                                            |
+----------------------------------------------+------------------+-------------+--------------------------------------------+
| DC-In Power Source Select (JPSEL1)           | 12V              | 2 - 3       |                                            |
+----------------------------------------------+------------------+-------------+--------------------------------------------+

Wiring
~~~~~~

+------------------------------+----------------+
| Connection To:               | Type:          |
+------------------------------+----------------+
| Backplane                    | Computer Power |
+------------------------------+----------------+
| Backplane                    | RS-232         |
+------------------------------+----------------+
| Backplane                    | RS-232         |
+------------------------------+----------------+
| PointGrey BlackFly Left      | USB 3.0        |
+------------------------------+----------------+
| PointGrey BlackFly Right     | USB 3.0        |
+------------------------------+----------------+
| PointGrey BlackFly Down      | USB 3.0        |
+------------------------------+----------------+
| LORD MicroStrain IMU-3DM-GX4 | USB 3.0        |
+------------------------------+----------------+
| Depth Sensor                 | USB 2.0        |
+------------------------------+----------------+

BIOS
~~~~

Press <ESC> or <DEL> to enter.


Boot Config
~~~~~~~~~~~

sudo nano /etc/default/grub

GRUB_CMDLINE_LINUX=”"

becomes:

GRUB_CMDLINE_LINUX=”text usbcore.usbfs_memory_mb=1000”

Uncomment:

#GRUB_TERMINAL=console

sudo update-grub


Main Housing Part 2
-------------------

Fasteners
~~~~~~~~~

                                                 add metric conversion

=================== ===== ======== ====== ======= ========== ==========
Mating              Count Material Thread Length  Torque     Coating
=================== ===== ======== ====== ======= ========== ==========
Forward Endcap      8     Nylon    8-32   0.875in 9in-lbs    Anti-Seize
Tension Rods        8     Krylon   8-32   0.5in   Hand-tight LOCTITE
Aft Endcap          8     Nylon    8-32   1.0in   9in-lbs    Anti-Seize
DVL Tube Cap        6     Krylon   8-32   0.875in 9in-lbs    Anti-Seize
Port I/O Panel      10    Nylon    8-32   1.0in   9in-lbs    Anti-Seize
Starboard I/O Panel 10    Krylon   8-32   1.0in   9in-lbs    Anti-Seize
Extension Latches   12    Nylon
=================== ===== ======== ====== ======= ========== ==========

Seals
~~~~~

============ ===== ====== ==== =============
Mating       Count Method Size Coating
============ ===== ====== ==== =============
Pressure     1     Twist?
Clear Tube   2     Gasket      None
Mid Housing  4     X-Ring      O-Ring Grease
DVL Tube Cap 1     Gasket      None
I/O Panels   2     Gasket      None
============ ===== ====== ==== =============

* Black Gaskets: Buna N 1/16" Thick (Formed from o-ring material.)
* See `Exterior Cables & Hoses`_ for SubConn connections.

Assembly
~~~~~~~~

.. warning::
   Ensure all fasteners attaching latches are tight and the sealing gasket appears compressed. DO NOT OVER TIGHTEN IF SECURED!

**Central Core:**

#. Place the DVL Tube Cap gasket on the tube.
#. Place the DVL cap on the DVL Tube Cap gasket.
#. Secure the DVL cap using 6 DVL Tube Cap fasteners.
#. Line up the 'ff' label on DVL with 'ff' label on housing for buoyancy.

.. note::
   For the time being the outermost rear fan bolts must be removed to insert and remove the electronics rocket.

#. Secure the pressure sensor wire out to the upper surface of the housing to prevent it from catch on the electronics rocket.
#. Insert (Land) electronics rocket from the forward side of the tube.

#. PUT THE O-RING ON THE PANEL THEN PUT THE SCREWS IN AND THEN PUT IT ON.

#. Place an I/O Panel gasket into the port mid housing receptacle. (Add link to panel chart.)
#. Place the Port I/O panel against the I/O panel gasket with the giant power SubConn on the forward side.

.. warning::
   Using a flashlight inspect the interior mating face to ensure the gasket is properly seated, repeat with finger.

#. Secure the Port I/O panel using 10 Port I/O Panel bolts by first applying anti-seize then finger-tightening them and then preceding  to do the star stuff. (Add links.)

.. warning::
   Ensure the I/O panel bolts pass through the electronics rocket without being forced, or they'll bend it and warp it.

REPEAT THE PORT PROCEDURE WITH THE STARBOARD SIDE...

#. Place the Starboard I/O Panel gasket into the starboard mid housing receptacle.
#. Place the starboard I/O panel atop the I/O panel gasket.
#. Secure the starboard I/O panel using [some fasteners].

**Backplane:**

* Add screws! Four, 4-40, 3/8", hand-tight, stainless

#. Bolt the backplane to the electronics rocket's four canty-lever rods using backplane screws and washers.
#. Connect all the cables.

**After Extension:**

Attaching the lid:

#. Clean the mating surfaces and gasket, ensuring to remove any excess anti-seize.
#. Place the gasket onto the housing mating surface and then place the lid onto the gasket.
#. For each of the 8 lid bolts, apply anti-seize and then insert the bolt about 3/4 of the way.
#. Tighten all bolts using the star pattern procedure.

Preparing the o-rings:

#. Clean out the o-ring housing grooves with cotton swabs, wash your hands or don gloves.
#. With clean hands squeeze a "pea and a schmear" sized amount of o-ring grease onto your thumb and forefinger.
#. Pull the o-ring through the grease while applying steady pressure to ensure the o-ring is evenly coated. (Perform 3 revolutions of the o-ring to ensure an even coating.)
#. Starting with the o-ring in contact with the aftermost groove, stretch the o-ring around the circumference of the tube and release it into it's slot.

.. warning::
   Check the o-ring to make sure it is not twisted.

#. Repeat for the second o-ring.

Inserting the tube:

#. Align the housing with the vehicle so that the latch tabs are horizontal.
#. Place the leading edge of the housing onto the after frame curved crossbar.
#. While being careful to avoid contact with the backplane, slide the housing forward until, it is within an inch of the central portion.
#. Slide the mating surfaces together, pushing firmly to engage the first o-ring.
#. Hook the latches over the latch tabs, and close them until the locks catch. Pull back to ensure successful locking mechanism engagement.
#. The housing is sealed if and only if both mating surfaces are now in full contact with one-another. (The upper portion will be more "in full contact" than the lower portion.)

**Forward Extension:**

Attaching the lid:

#. Clean the mating surfaces and gasket, being careful to remove excess anti-seize.
#. Place the gasket onto the housing mating surface and then place the lid onto the gasket.
#. For each of the 8 lid bolts, apply anti-seize and then insert the bolt about 3/4 of the way.
#. Tighten all bolts using the star pattern procedure.

Preparing the o-rings:

#. Clean out the o-ring grooves with cotton swabs, wash your hands or don gloves.
#. With clean hands squeeze a "pea and a schmear" sized amount of o-ring grease onto your thumb and forefinger.
#. Pull the o-ring through the grease while applying steady pressure to ensure the o-ring is evenly coated.
#. Starting with the o-ring in contact with a groove stretch the first o-ring around the circumference of the tube and release it into it's slot.

.. warning::
   Check the o-ring to make sure it is not twisted.

#. Repeat for the second o-ring.

Inserting the tube:

#. Align the housing so that the latch tabs are horizontal.
#. Place the leading edge of the housing onto the forward frame curved crossbar.

#. Tilt the housing forward until the lower leading edge is low enough to pass below the downward-facing camera.
#. Push the housing longitudinally for an inch before leveling the housing.

#. While being careful to avoid contact with the camera, slide the housing aft until, it is within an inch of the central portion.
#. Slide the mating surfaces together, pushing firmly to engage the first o-ring.
#. Hook the latches over the latch tabs, and close them until the locks catch. Pull back to ensure successful locking mechanism engagement.
#. The housing is sealed if and only if both mating surfaces are now in full contact with oneanother.


Mounting
~~~~~~~~

**Attaching Central Core to Frame**

**Attaching Forward Extension to Central Core**

See above, for now.

**Attaching After Extension to Central Core**

See above, for now.

Main Housing
------------

.. warning::
   Careful not to twist or tear O-rings during assembly
   Visually check the mating interfaces have a uniform gap

Fasteners
~~~~~~~~~
Back cap: #8 screws

Front Cap Assembly
~~~~~~~~~~~~~~~~~~
.# Place the front cap bottom stainless steel rods in the channels.
.# Line up the sealing surfaces.
.# Engage latches by carefully forcing front cap into main housing.
.# Pull latches at the same time to fully close the front of the vehicle.

Back Cap Assembly
~~~~~~~~~~~~~~~~~
.# Attach the Acrylic plate to rear end of the Aluminum tube.
.# Place the #8 screws on the aluminum ring through the acrylic plate.
.# Place the gasket on all the screws.
.# Torque screws to 9 in-lb in a star pattern.
.# Lube 2 X-profile Bruna-N 265 O-Rings and place in O-Ring grooves.
.# Slide the back cap around the backplane.
.# Line up the sealing surfaces.
.# Engage latches by carefully forcing front cap into main housing.
.# Pull latches at the same time to fully close the front of the vehicle.
