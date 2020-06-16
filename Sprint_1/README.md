RCOMP 2019-2020 Project - Sprint 1 - Member 1181444 folder
===========================================
(Tiago Soares Ribeiro)

-----------------------------------------------------------

### Building C ###

##### Rooms Area Measurements:

* Floor Zero:

	* Total Area : (80m * 30m) = 2400 m 2
	* Right Area : (60m * 30m) = 1600 m 2
	* Left Area : (20m * 30m) = 800 m 2
	* Room CO.1 : (7,5m * 6m) = 45 m 2
	* Room CO.2 : (7,5m * 6m) = 45 m 2
	* Room CO.3 : (7,5m * 6m) = 45 m 2
	* Room CO.4 : (8m * 5,5m) = 44 m 2
	* Room CO.5 : (6m * 5,5m) = 33 m 2

	* Floor Zero Common Area (Hall, WC’s, Stairs): 2400 m 2 – 1812 m 2 = 588 m 2
	
* Floor One:

	* Left Area : (20m * 30m) = 800 m 2
	* Room C1.1 : (6m * 7m) = 42 m 2
	* Room C1.2 : (6m * 7m) = 42 m 2
	* Room C1.3 : (6m * 11m) = 66 m 2
	* Room C1.4 : (5,5m * 15m) = 82,5 m 2
	* Room C1.5 : (5,5m * 13m) = 71,5 m 2

	* Floor One Common Area (Hall, WC’s, Stairs): 800 m 2 - 304 m 2 = 496 m 2

##### Resulting standard number of network outlets:

* Floor Zero:
 
	* Ground Floor Right Area : (2 + (1600 / 10)*2) = 322 outlets (ISO8877 / RJ45)
	* Room CO.1 : (2 + (45 / 10)*2) = 13 outlets (ISO8877 / RJ45)
	* Room CO.2 : (2 + (45 / 10)*2) = 13 outlets (ISO8877 / RJ45)
	* Room CO.3 : (2 + (45 / 10)*2) = 13 outlets (ISO8877 / RJ45)
	* Room CO.4 : (2 + (44 / 10)*2) = 11 outlets (ISO8877 / RJ45)
	* Room CO.5 : (2 + (33 / 10*2) = 9 outlets (ISO8877 / RJ45)
	
* Floor One:

	* Room C1.1 : (2 + (42 / 10)*2) = 10 outlets (ISO8877 / RJ45)
	* Room C1.2 : (2 + (42 / 10)*2) = 10 outlets (ISO8877 / RJ45)
	* Room C1.3 : (2 + (66 / 10)*2) = 15 outlets (ISO8877 / RJ45)
	* Room C1.4 : (2 + (82,5 / 10)*2) = 18 outlets (ISO8877 / RJ45)
	* Room C1.5 : (2 + (71,5 / 10*2) = 16 outlets (ISO8877 / RJ45)

-----------------------------------------------------------


##### Schematic Plans:

####### Floor Zero :

-----------------------------------------------------------

![Floor Zero](C_floor_0.png)

-----------------------------------------------------------

With the calculations seen above, the number of network outlets was respected according to the standard, being deployed two for each 10 m 2 , and adding 2 to the room in assessment. 
The schematic plan of network outlets of the left work area depicted in the image above, shows
a care for placement in a manner that one user has always an available outlet in a 3 meter radius.
Regarding the right area, the outlets were directly attached to the suspended cable raceways in
order to provide a homogenous coverage of the entire open space, they were spread in each
vertical railway in sets of 7, totalling 28 for each railway, and sets of 4 in each vertical railway
interval. This way, they are not overly cluttered, and they provide some free space in the railway
for easier access and possibly technician manoeuvering.

Due to the massive surface covered with network outlets in the right area, 10 consolidation
points were added where each one handles the vertical cable raceway at his right and the 4
outlets on horizontal raceway, also at it’s right, in order to control the cable sizing. This way,
another rule of horizontal cabling is fulfilled, which is that in a straight line, no cable is ever
longer than 90 meters, and in a straight line, the distance of an HC to any outlet is not greater
than 80 meters.

Regarding wireless access points, since they provide a somewhat reliable service in a radius of
30 meters, 3 devices were deployed across the floor respecting this feature, allowing a full
coverage of the area, with the necessary overlaps, to compensate the possible disturbance of
the signal propagation due to walls or columns.

Backbone wise, to respect an important rule of structured cabling that states that a horizontal
cross-connect should never cover an area of 1000 m 2 or larger. Since the right work area alone
has 1600 m 2 , two HC’s were added to the room, each one controlling essentially half of it. In the
left area, one HC is enough. As seen in the image, the right HC (1) is the one handling the CP’s
and Access Point with the number 1 on them, the same applies to HC (2) and HC (3), following
the same logic. To facilitate access, and adding logic, the Intermediate cross-connect of this
building is located in the same room as the external ditch entry.

-------------------------------------------------------------

####### Floor Zero :

Since the right 1600 m2 area of the building is common to both floors, the following blueprint
only depicts the left area of the first floor, since the right area was shown above in the ground
floor blueprint.

![Floor One](C_floor_1.png)

-----------------------------------------------------------

Like the below floor, outlets were placement following the same logic, allowing any user to have
an outlet within roughly 3 meters. To facilitate cable management and possible upgrades,
consolidation points were added to this area aswell, one handling the C1.5 room because it is
distanced from the upper rooms, another one handling the C1.4 room, and finally one handling
C1.2 and C1.3 rooms.

To facilitate access, and adding logic, the Intermediate cross-connect of this building is located
in the same room as the floor cable passageway. A wireless access point was also added covering
the entire area.

All horizontal cabling rules were accomplished, with no cable being greater than 90 meters, the
area covered by the horizontal cross-connect is tasked with handling 800 m 2 , and in a straight
line, the distance from the HC/CP is far less than the recommended 80 meters.

-----------------------------------------------------------

##### Cabling:

The used cable is CAT6 as solicited in the Laboratory Class 01 Sprint guidelines. Types above are
significantly more expensive, and the CAT6 can handle perfectly the task at hands in this Sprint.
It follows the T568A wiring pattern across the entire blueprint.

-----------------------------------------------------------

##### Cabling Measures (Floor Zero):

**Room C0.1** longest cable has 12,5 meters (the one feeding the access point of the left area work
area) and the smallest one has 3 meters, which feeds the outlet nearest of the HC. Making an
average of 7,75 meters. Since there are 14 cable connections there + 1 for redundancy between
backbone cabling, this room needs **117** meters of cable.

**Room C0.2** longest cable has 16,5 meters (the one feeding the bottom left outlet of the room)
and the smallest has 5,5 meters, which feeds the top right outlet. Making an average of 11
meters. Since there are 14 cable connections aswell + 1 for redundancy between backbone
cabling, this room needs **165** meters of cable.

**Room C0.3** longest cable has 12,5 meters (the one feeding the bottom right outlet of the room)
and the smallest has 2,5 meters, which feeds the top left outlet. Making an average of 7,5
meters. Since there are 15 cable connections + 2 for redundancy between backbone cabling, this
room needs **128** meters of cable.

**Room C0.4** longest cable has 29 meters (the one feeding the bottom left outlet of the room) and
the smallest has 20 meters, which feeds the top right outlet. Making an average of 24,5 meters.
Since there are 11 cable connections, this room needs **270** meters of cable.

**Room C0.5** longest cable has 21 meters (the one feeding the bottom right outlet of the room)
and the smallest has 13 meters, which feeds the top left outlet. Making an average of 17 meters.
Since there are 9 cable connections, this room needs **153** meters of cable.

**Right Area** longest cable has 29 meters (the one connecting both horizontal cross-connects of
the area) and the reasonably smallest has 1,5 meters, which is any cable connecting a
consolidation point to the outlet on the right. Making an average of 15,5 meters. Since there are
332 cable connections, this area needs **5146** meters of cable.

The ground floor needs roughly **6000** meters of cable.

-----------------------------------------------------------

##### Cabling Measures (Floor One):

**Room C1.1** longest cable has 24 meters (the one feeding the access point of this floor) and the
smallest has 1,5 meters, which feeds the outlet nearest of the horizontal cross connect. Making
an average of 13 meters. Since there are 12 cable connections, this room needs **156** meters of
cable.

**Room C1.2** longest cable has 19 meters (the one feeding the bottom right outlet of the room)
and the smallest has 1,5 meters, which feeds the outlet right to the consolidation point. Making
an average of 11 meters. Since there are 10 cable connections + 2 for redundancy between
backbone cabling, this room needs **132** meters of cable.

**Room C1.3** longest cable has 29 meters (the one connecting the bottom right outlet to the
second room consolidation point), and the smallest has 11 meters, which feeds the top right
outlet of the room. Making an average of 20 meters. Since there are 13 connections + 2 for
redundancy between backbone cabling, this room needs **300** meters of cable.

**Room C1.4** longest cable has 24,5 meters (the one connecting both consolidation points), and
the smallest has 3 meters, which is the one connecting the adjacent consolidation point and
the nearest outlet to it. Making an average of 14 meters. Since there are 18 cable connections
+ 2 for redundancy between backbone cabling, this room needs **252** meters of cable.
 
**Room C1.5** longest cable has 19 meters of cable (the one feeding the bottom left outlet of the
room), and the smallest has 5 meters, which is the one feeding the top right outlet. Making an
average of 12 meters. Since there are 16 cable connections, this room needs **192** meters of
cable.

The upper floor needs roughly **1050** meters of cable.

-----------------------------------------------------------

##### Total:

* The total length of cable needed is roughly 7050, which we’ll round up to **7100** for safety.

-----------------------------------------------------------

##### Inventory:

* CAT6 Cable – 7100 meters
* RJ45 Outlets – 450 units
* 48 Set Patch Panels – 24 (oversize considered)
* 24 Set Patch Panels – 10 (oversize considered)
* Enclosures for CP’s - 15
* Enclosures for HC’s - 4
* Enclosures for IC’s – 1
* Access Point Hardware - 4