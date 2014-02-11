Camel SMB Component
===================
This project is a Samba Camel component build on top of JCIFS (http://jcifs.samba.org/).

It was originally developed by Redpill Linpro AB and Helsingborgs stad as part of a integration project.

This component is licensed under the LGPL (http://www.gnu.org/licenses/lgpl-2.1.txt)

The unit testing is done by mocking out the jcifs library to be able to run automaticly.

There are some manuell integration tests (src/integrationtest) that are meant to be run with a a 
local CIFS server (Samba or MS Windows share).
To run these copy camelsmb.prp.template to your home directory, rename it to camelsmb.prp" and edit 
to include correct details.

Contributor
-----------
Martin Samuelsson [martin __AT__ martsam __DOT__ se]  
Pontus Ullgren [ullgren gmail com]

Build
-----

To build use this command: mvn clean install

To deploy to nexus use: mvn clean deploy

To build faster use -Pfastinstall
