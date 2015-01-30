maven-archetypes
================

This repository will hold a variety of maven archetypes that use JBoss middleware in configurations tailored for large, enterprise projects.

Archetype Build Instructions
------------------------------
To build an archetype on the command line, change directory (cd) to the parent project directory.

1. cd $YOUR_PROJECT
1. mvn archetype:create-from-project
1. cd target/generated-sources/archetype
1. mvn install

On successful build, maven will create a parent-archetype folder under the com.rhc group in M2_REPO.  Maven will also generate a local catalog (archetype-catalog.xml) in the M2_REPO folder.

1. In JBoss Developer Studio, File->New->Maven Project
1. When prompted to choose an archetype, click Configure
1. Click Configure->Add Local Catalog
1. Select the local catalog in the M2_REPO and click Include Snapshots on the selection page
1. Select the parent-archetype and click Finish
