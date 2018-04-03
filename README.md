# Mounting Extender Nodes

_work in progress_

Also, see https://sudoroom.org/wiki/Mesh/Mounting .

Related to all things mounting - equipment, prep, knowledge sharing.

* [Questions to ask at the very beginning](#questions-to-ask-at-the-very-beginning)
* [Scouting the location](#scouting-the-location)
* [Planning the Mount and Establishing Consent](#planning-the-mount-and-establishing-consent)
* [Flashing Routers](#flashing-routers)
* [Prior to Mounting](#prior-to-mounting)
* [Actually On Site](#actually-on-site)

## Questions to ask at the very beginning

* Where do you want to mount your extender node? Do you know what you are aiming at? Do you know of any nearby PON nodes?
* Do you have a group of people to do the mount with? Ideally between two and four people, with at least one having done an install before.
* Have you had any safety training? At the least, brush up on [OSHA guidelines](https://www.osha.gov/law-regs.html), especially [the ladder section](https://www.osha.gov/pls/oshaweb/owadisp.show_document?p_table=STANDARDS&p_id=9715).
* Did you look up the location in publicly available GIS and LIDAR data (i.e. Google Earth/Maps and https://link.ubnt.com/)?

## Scouting the location

* Do you have a contact on site, and are they available?
* Do you have roof access? Are there any local zoning or home owners associate considerations?
* Is there actually a good place to mount the antenna?
* Can you actually see the node you are aiming for? Line of sight is key!
  * Easy check: can you see a `peoplesopen-node2node` ssid?
  * Consider pointing to future node mount location using [azimuth calculator](https://www.fcc.gov/media/radio/distance-and-azimuths).
* Discuss the mounting process with the contact (see below.)
* Make sure contact information is exchanged so you can coordinate the actual install at a future time.
* Plot your anticipated cable run.

## Planning the Mount and Establishing Consent

It's important to establish consent for the various components of the installation with the node operator.

Mounting options are primarily limited by *line of sight* and *building architecture*.

* *Do not create a hole in the roof.*
* Ideally, mount to a wall with a J-pole or strut and mast, or mount to a sturdy vent pipe with hose clamps.
* The operator and neighbors might also be concerned with the visibility of the antenna - from the street, from neighboring homes, etc.
* Don't just get line of sight to a node for an uplink; try to maximize the potential for future nodes to have line of sight to the one you're mounting.

When determining the wire run, consider the following:

* Minimizing the length of the run. Where is the extender node going, and where is the home node going?
* Minimizing the probability of anyone tripping over the cable.
* Securing the cable to prevent it from becoming a tripping hazard, dropping from the roof, etc.

That said, be sure to discuss this with the node operator.
If they don't want the cable to pass through a wall, consider their suggestions.
If you don't feel comfortable proceeding with the run due to
safety, time constraints, risk of damaging the building, or risk of damaging the equipment,
the operator can take responsibility for that component.

* *Again, do not create a hole in the roof.*
* Be sure to properly seal any penetrations with liberal application of caulk. If the weather is wet, use a quick-setting caulk.

## Flashing Routers

* Always flash the routers prior to getting on site. If possible, run `makenode` prior to getting on site.
* Make sure you have the right power adapter for what you are installing!
* Follow the [walkthrough](https://peoplesopen.net/walkthrough).
* Flash backup equipment if possible. Always good to have a spare to save a potential second (Well, third if you count the scouting trip) visit.

## Prior to Mounting

* Do you have all your [tools](https://sudoroom.org/wiki/Mesh/Mounting#Tools)?
  * Cat5 crimps and crimpers
  * Cat5 cable (at least 100')
  * Cable tester
  * A drill with bits suitable for what you will be putting holes in
  * Mounting hardware suitable for your surface. Mounting on wood or asbestos is different from mounting on concrete or stucco.
  * Whatever you need (caulk, grommets, etc) to seal any penetrations involved in mounting the node and running cable
  * Spare extender / home node with power supplies
* Do you have necessary safety [equipment](https://sudoroom.org/wiki/Mesh/Mounting#Safety_Equipment)?
* Make sure you will have a contact on site.
* Review relevant safety guides

## Actually On Site

* With four people you can have two doing the actual install, one person acting as a spotter for safety hazards, and a fourth interacting with the contact on site.
  * At least one person should have done this before.
  * At least one person should have been on the scouting trip.
* If a plan was previously established on a scouting trip, review it with the node operator and reestablish consent before proceeding.
* Test equipment before mounting it. Battery powered PoE injectors can be helpful here.
  * This goes for both the extender and mesh nodes.
* Confirm the actual cable run. Never put holes in a roof for cables always in a wall.
  * Keep in mind max cat5 lengths. Generally aim for 300' max.
  * Make sure to use shielded/grounded cable outside.
  * Leave a "drip loop" where the cable goes into the building. This is a downward curve of the cable which helps water not enter the building.
  * If desired by site contact, you can use conduit or panduit for aesthetics.
* If you will be crawling around in attics you may wish to have a respirator.
* When mounting extender nodes, the POE sheath should be pointing down. This will ensure the LED's are not pointing up, as they apparently attract birds.
* Exchange contact information with the site contact before leaving.
