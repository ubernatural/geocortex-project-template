# Geocortex Items Directory
Place exported geocortex items in subfolders in this directory, according to the following structure:  
  
gxp: Geocortex Printing templates
gxr: Geocortex Reporting templates
gxw: Geocortex Web layouts and templates
gxwf: Geocortex Workflows

If a project does not have any of a particular item, exclude the folder. As in, do not have any empty folders - it's confusing.

Ensure that the formatting of the items (those which are json) is consistent; that is, the indentation and line break settings must match those of Geocortex Item Manager (the standard). The reason for formatting the items is to make it possible to view diffs between versions.

See below for a description of what should be saved in each folder, and in what format.

## Geocortex Printing Templates
TODO

## Geocortex Reporting Templates
TODO

## Geocortex Web Layouts and Templates
TODO

## Geocortex Workflows
Geocortex Workflows are saved in the gxwf folder. At a minimum this should be the Workflow itself in formatted json. Workflows which are client-side can be copied, already formatted, from Geocortex Item Manager or from Esri's ago-assistant. Both server and client Workflows can be exported from GXWF Designer, but must be formatted afterwards.

The naming convention of the items in this folder is `Workflow Name.json`. This is what is exported from GXWF Designer by default. Spaces in the name are fine, since the name of this file will translate into the name of the item in AGOL/Portal and should be human-readable.

You _should_ also include a json file with details of the portal item itself. This can be exported from Geocortex Item Manager or Esri ago-assistant, though it is not exportable through GXWF Designer. This file includes tags, properties, portal item description, and other details which are valuable to maintain a record of.

Do not use the gxwf folder to store custom Workflow Activities / Form Elements - those are developed in the top level activity-pack directory.