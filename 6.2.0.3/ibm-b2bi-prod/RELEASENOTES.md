# What's new in Helm Charts Version 3.0.5 for IBM Sterling B2B Integrator Enterprise Edition v6.2.0.3
* Support for ITX and ITXA integration on a container deployment
* New document service component as an add-on sub chart deployment to support Object Store as a document payload storage option
* Support for rebranding SFG User Interfaces using Customization UI
* Support for Azure SQL Managed Instance
* Support for rolling upgrades from v6.1.0.x.
* Tech stack upgrades
    Red Hat UBI base image version 9.4.x
    Red Hat OpenShift Container Platform 4.14, 4.15 and 4.16 or later fixes
    Kubernetes versions >=1.28 and < =1.30
    Helm version 3.15.x

# Breaking Changes
Rolling upgrades for product version v6.1.0.x will be supported but for product versions earlier than v6.1.0.0 installed using IIM, Docker or Certified Container will not be supported.

# DB Changes (refer Version History section below)
If its fresh install =>
	Set dataSetup.enabled to true and dataSetup.upgrade to false in values.yaml
In case of upgrade =>
	If DB Changes are introduced, then set dataSetup.enabled to true and dataSetup.upgrade to true
	If DB Changes are not introduced, then set dataSetup.enabled to false and dataSetup.upgrade to true


# Documentation
Check the README file provided with the chart for detailed installation instructions.

# Fixes
N/A

# Prerequisites
Please refer prerequisites section from README.md

# Version History

| Chart | Date | Kubernetes Version Required | Breaking Changes | Details | DB Changes |
| ----- | ---- | --------------------------- | ---------------- | ------- | ---------- |
| 2.0.1   | December 18, 2020 | >=1.14.6 | N  | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | N | 
| 2.0.2   | March 19, 2021 | >=1.14.6 | N  | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | N |
| 2.0.3   | June 29, 2021 | >=1.17 | N  | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | N |
| 2.0.4   | Novemeber 10, 2021 | >=1.17 | N  | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | N |
| 2.0.5   | January 14, 2022 | >=1.17 | N  | iFix release upgrade for IBM Sterling B2B Integrator Certified Containers | N |
| 2.0.6   | May 13, 2022 | >=1.17 | N  | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | N |
| 2.0.7   | July 07, 2022 | >=1.17 | N  | iFix release upgrade for IBM Sterling B2B Integrator Certified Containers | N |
| 2.1.0   | Sep 30, 2022  | >=1.21 | N | Mod release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
| 2.1.1   | Dec 16, 2022  | >=1.21 | N | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
| 2.1.2   | Mar 03, 2023  | >=1.23 | N | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
| 2.1.3   | Mar 27, 2023  | >=1.23 | N | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
| 2.1.4	  | July 15, 2023 | >=1.23 | N | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
| 3.0.0   | Sept 22, 2023 | >=1.25 | N | Major release upgrade for IBM Sterling B2B Integrator Certified Containers      | Y |
| 3.0.1   | Mar 31, 2024 | >=1.26 | N | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
| 3.0.4   | Jun 7, 2024 | >=1.27 | N | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
| 3.0.5   | Aug 31, 2024 | >=1.27 | N | Fix pack release upgrade for IBM Sterling B2B Integrator Certified Containers | Y |
