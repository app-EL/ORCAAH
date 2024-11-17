# ORCAAH
 Optical Reef and Coastal Area Assessment of Hawaii Tool

===============
============================================================================================================
Optical Reef and Coastal Area Assessment of Hawaii (ORCAAH) Tool
============================================================================================================
===============

Date Created: August 26, 2024

The Optical Reef and Coastal Area Assessment of Hawaii (ORCAAH) tool is a fork of the NASA DEVELOP Optical Reef and Coastal Area Assessment (ORCAA) Tool.

Settings have been changed to meet the specific needs of Hawaii nearshore environnments and reef systems

It allows users to monitor, track, and evaluate water parameters in Hawaii Island nearshore reefs from January 2013 through the current date.

It uses a graphical user interface (GUI) so that users can easily add, process, view, and export data. The interface contains four main parts:

        1. a panel to set analysis parameters (time range and area of analysis)
        2. a panel to select analysis types and add images to the map
        3. a panel to export images to Google Drive
        4. a time series chart generator that creates line graphs based on the selected time range, area of analysis, and water quality parameter of interest 

Based on the user selected time range and area of analysis, the tool accesses and filters Landsat 8 Level 2 Surface Reflectance, Sentinel-2 Level 1C, Aqua MODIS, and Terra MODIS collections to create cloud-masked and land-masked collections. The Sentinel-2 collection is also run through the Modified Atmospheric correction for INland waters (MAIN) algorithm developed by Benjamin Page at the University of Minnesota, Twin Cities to atmospherically correct the Sentinel-2 coastal imagery. 

Turbidity, Normalized Difference Chlorophyll Index, chlorophyll-a concentration, and colored dissolved organic matter concentration are calculated from the filtered and corrected Sentinel-2 image collection. Turbidity is also derived from the filtered Landsat 8 collection. Sea surface temperature is taken from the ‘SST’ band in the MODIS collections. 

===================
 Required Packages
===================

ORCAAH derives all analyses using Google Earth Engine's free and publicly accessible data catalog.
Users do not need to load in their own data, but do need to request an account with Google Earth Engine at code.earthengine.google.com.
Accounts are free and typically approved within a few days. 

============
 Parameters
============

No steps must be taken to modify the code to enable it to run - users paste the provided code directly into the Google Earth Engine Code Editor and
select "Run." This will load the interface with which users directly interact. The interface includes brief directions to guide users through each analysis option. 

======================
 Contact ORCAAH Tool
======================

Names: Erik Lash
E-mails: erik.lash@hawaiicounty.gov

==================================
 Contact NASA DEVELOP ORCAA tool
==================================

Names: Vanessa Valenti | Hayley Pippin | Arbyn Olarte | Roxana Pilot
E-mails: vvalenti@ucla.edu | habpippin@berkeley.edu | arbynolarte@gmail.com | roxana.pilot@gmail.com

============================
 Copyright Notice
============================
This software may be used, reproduced, and provided to others only as permitted under the terms of the agreement under which it was acquired from the U.S. Government.  Neither title to, nor ownership of, the software is hereby transferred.  This notice shall remain on all copies of the software.

Copyright 2020 United States Government as represented by the Administrator of the National Aeronautics and Space Administration. All Rights Reserved.