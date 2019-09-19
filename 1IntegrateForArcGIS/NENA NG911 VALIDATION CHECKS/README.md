# NENA NextGen911 Validation Checks
This repository includes sample 1Integrate for ArcGIS validation checks against the National Emergency Number Association (NENA) [NG9-1-1 GIS Data Model](https://www.nena.org/page/NG911GISDataModel) created on 06/16/2018.

For instructions on uploading and publishing Rulesets, please refer to the following [documentation](https://1spatial.com/documentation/1integrate-arcgis/v2/Topics/Rules/Free_Rulesets.htm).

## Repository Structure
This repository folder is broken down by layer identified within the NENA guidelines.  It includes all the Validation rules for that layer, including Conditional, Mandatory and Optional Rules, as defined in the NENA guidelines. 

## NENA NG911 Validation Checks
### [NENA NG911 Validation Checks](NENA_Validations.rules)
In lieu of Valid Values tables, the validation rules that reference them have been flagged with a comment to revise the string as necessary, particularly values that indicate state abbreviation and county names. The current ruleset uses the state of Maryland as an example. The abbreviation "US" has been populated as a default Country value.

## Template Schema
The template schema folder contains an Esri File Geodatabase of the expected NENA Schema along with a packaged project file containing it created in ArcGIS Pro v2.4.1. To ensure compatibility between your data and these rules, the folder also includes a JSON file to be uploaded and referenced as a schema on the 1Integrate for ArcGIS Rule Author. For instructions on managing schemas, please refer to the following [documentation] (https://1spatial.com/documentation/1integrate-arcgis/v2/Topics/Rules/Schemas.htm).

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
