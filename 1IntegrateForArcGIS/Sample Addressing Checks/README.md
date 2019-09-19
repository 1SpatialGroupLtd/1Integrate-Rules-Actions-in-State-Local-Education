# Sample Addressing Checks
This repository folder contains some Sample Addressing Checks that can be used with 1Integrate for ArcGIS.
These addressing checks are used by a number of State and County organizations using 1Spatial's 1Integrate for ArcGIS software. 
These rules are written against the NENA NextGen911 Standard Schema for Road Centerlines and Site Structure Address Points.
For instructions on uploading and publishing Rulesets, please refer to the following [documentation](https://1spatial.com/documentation/1integrate-arcgis/v2/Topics/Rules/Free_Rulesets.htm).

### [Sample Addressing Checks](SampleAddressingChecks.rules)
Listed below are descriptions and syntax of each individual rule contained within the sample ruleset.

## Road Centerline Validation Checks

### Road Centerline has no gaps in address range
Checks that there are no gaps in the address range between conecting road centerlines with the same road name.  The address gap should only be 2 addresses.  For example if Centerline A has an address range of 2 to 50 then centerline B must have a from address of 52.
This check only looks at roads that are connected from a start to end relationship.
![Alt text](img/CenterlineAddressesHaveNoGaps_Rule.png?raw=true "Centerline Address Range Gap Rule Screenshot")

### Road Centerline has no overlapping addresses
Checks that there are no overlap in the address range between conecting road centerlines with the same road name.  
This check only looks at roads that are connected from a start to end relationship.
![Alt text](img/CenterlineAddressesHaveNoOverlaps_Rule.png?raw=true "Centerline Address Range Overlap Rule Screenshot")

### Road Centerline address Parity Switch Check
Checks that if two roads are connected at either the start or the end that both road centerline left address ranges have either even or odd addresses and are not mixed.


## Site Address Point Validation Checks
### Site Address Point has matching street name
Checks that every address point has a road centerline within 200 units (typically feet or meters depending on the coordinate system) that has the same road name.
![Alt text](img/SSAPHasCenterlineWithSameName_Rule.png?raw=true "SSAP vs Centerline Street Name Rule Screenshot")

### Site Address Point has matching full street name
Checks that every address point has a road centerline within 200 units (typically feet or meters depending on the coordinate system) that has the same road name, road type (pre and post), road direction (pre and post), etc.
![Alt text](img/SSAPHasCenterlineWithSameStreetAttributes_Rule.png?raw=true "SSAP vs Centerline Street Attributes Rule Screenshot")

### Site Address Point is within matching PSAP Boundary
Checks that every address point is within a PSAP Boundary and the PSAP_ID of the address point matches the PSAP_ID of the PSAP that the address point is within.
![Alt text](img/SSAPWithinCorrectPSAP_Rule.png?raw=true "SSAP Within Correct PSAP Rule Screenshot")


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