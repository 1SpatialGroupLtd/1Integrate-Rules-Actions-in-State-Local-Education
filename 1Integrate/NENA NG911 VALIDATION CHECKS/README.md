# NENA NextGen911 Validation Checks
This repository includes sample 1Integrate validation checks against the National Emergency Number Association (NENA) [NG9-1-1 GIS Data Model](https://www.nena.org/page/NG911GISDataModel) created on 06/16/2018.

For instructions on restoring a backup please refer to the following [documentation](https://1spatial.com/documentation/1integrate/v2_5/Topics/Backup_Restore.htm?Highlight=Restore%20Backup%20Rules)

## Repository Structure
This repository folder is broken down by layer idenified within the NENA guidelines.  Each XML file includes all the Validation rules for that layer, including Conditional, Mandatory and Optional Rules, defined in the NENA guidelines. There are also helper DataStore backups that will assist in getting your 1Integrate environment configured.

## Required Layers
### [Emergency Service Boundary](RequiredLayers\Emergency_Service_Boundary.xml)
### [Provisioning Boundary](RequiredLayers\Provisioning_Boundary.xml)
### [PSAP Boundary](RequiredLayers\PSAP_Boundary.xml)
### [Road Centerline](RequiredLayers\Road_Centerline.xml)
### [Site Structure Address Point](RequiredLayers\Site_Structure_Address_Point.xml)

## Strongly Recommended Layers
### [Complete Landmark Name Alias Table.xml](StronglyRecommendedLayers\Complete_Landmark_Name_Alias_Table.xml)
### [Counties](StronglyRecommendedLayers\Counties.xml)
### [Incorporated Muni Boundary](StronglyRecommendedLayers\Incorporated_Muni_Boundary.xml)
### [Landmark Name Part Table](StronglyRecommendedLayers\Landmark_Name_Part_Table.xml)
### [Neighborhood Comm Boundary](StronglyRecommendedLayers\Neighborhood_Comm_Boundary.xml)
### [States](StronglyRecommendedLayers\States.xml)
### [Street Name Alias Table.xml](StronglyRecommendedLayers\Street_Name_Alias_Table.xml)
### [Unincorporated Comm Boundary.xml](StronglyRecommendedLayers\Unincorporated_Comm_Boundary.xml)

## Recommended Layers
### [Cell Site Location](RecommendedLayers\Cell_Site_Location.xml)
### [Hydrology Line](RecommendedLayers\Hydrology_Line.xml)
### [Hydrology Polygon](RecommendedLayers\Hydrology_Polygon.xml)
### [Mile Marker Location](RecommendedLayers\Mile_Marker_Location.xml)
### [Railroad Centerline](RecommendedLayers\Railroad_Centerline.xml)

## TemplateDataStore
The template datastore folder includes a 1Integrate backup of a DataStore that matches the NENA Schema and another DataStore that holds the Valid Value lists (Domain Lists) for Country, State & County names.  Also included are Esri File Geodatabases of the expected NENA Schema and the Valid Values tables.      
The Valid Values datastore will be required to run some of the validation checks.  The NENA schema database, can help organizations migrate their data into that schema.

## Licensing
Copyright © 2018 1Spatial US Patent Number 9542416 B2 (2017-01-10)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's [license.txt](LICENSE) file.
