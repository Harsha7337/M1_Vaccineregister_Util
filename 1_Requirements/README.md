# REQUIREMENTS    
# Introduction
The deployment of covid-19 vaccines in India was done in a sudden burst and thus the tracking became very complicated. Due to multiple input and output commands on the server, it resulted in several slow running issues and crashes. The Aadhar details were used to allot the vaccines and hence it operated on a central server. To avoid the use of central server for all commmands, a local server will be loaded with the vaccine-registered data. Local verification and completion of vaccination data will be processed locally and will be loaded back to the main server by the end of day.

The local server must store the data of around 100 people where the allocated online registration data will be loaded onto the local server of that local centre. 
Verification of the data is done based on the details provided by the patient. Once completed, the data of the vaccinated will be sent back for future use and reference.
### Advantages
* Smoother data handling.
* Pre data readily available for verification.
* Flexibility to  add new  registrations limited with server alloted memory.
### Disadvantages
* Cannot add large number of new registrations due to local server limitations.
* Encryption is not enabled to protect the data.
* OTP verification is  not activate for new registrations.

# State of art/Research #

![vaccine (1)](https://user-images.githubusercontent.com/98849090/153673830-21fb6e06-bd13-4e46-987a-bea4fe0235b0.jpg) ![vaccine (2)](https://user-images.githubusercontent.com/98849090/153674034-bc67d7dd-965b-49df-9f3e-49c95ff9f460.jpg)


Each vaccine centre will operate locally to register and allot vaccines. The basic registration can be done online and schedules are set as desired by the patient. Assuming a vaccination centre can vaccinate around 100 people in a day. The data handling for online basic registration will be mostly done in the day time and the data acquired by the local centres of vaccinated people can be handled in the night.

The local server must store the data of around 100 people where the allocated online registration data will be loaded onto the local server of that local centre. Verification of the data is done based on the details provided by the patient. Once completed, the data of the vaccinated will be sent back for future use and reference.

## SWOT Analysis

![SWOT analysis](https://user-images.githubusercontent.com/89698000/132556785-561d19ab-c53d-4658-8138-401da25ce78e.png)

## 4 W's and 1 H
### Who
* Patient who needs to be vaccinated.
### What
* Verify the details of the patient using the alloted data.
### When
* During the time alloted for vaccination.
### Where
* Local vaccination centre.
### How
* Online registration and on field verification using local server.

## High Level Requirements
| ID | Description | Status (Implemented/Future) |
| --- | --- | --- |
| HR01 | System should be able to access pre loaded registration data for verification | Implemented |
| HR02 | User should be able to add new registrations | Implemented |
| HR03 | System should recognize vaccinated patients | Implemented |
| HR04 | System should recognize invalid credentials | Implemented |
| HR05 | System should be updated with the time interval between two doses | Future |
| HR06 | OTP generated verification for secure registration | Future |
| HR07 | System should recognize invalid credentials | Future |
| HR08 | System  send alert SMS to upload nearby covid attack patient | Future |


## Low Level Requirement
| ID | Description | Status (Implemented/Future) |
| --- | --- | --- | 
| LR01 | Only new user must be given an option to select vaccine type | Implemented |
| LR02 | Total quantity of vaccines used must be shown by EOD | Implemented |
| LR03 | Full list of patients vaccinated must be set as output | Implemented |
| LR04 | Remaining and present stock of vaccines must be tracked | Future |
| LR05 | 1st dose Vaccinated patient get notify with an SMS to get regester for the 2nd dose   | Future |
| LR06 | Virtual chat bot is added to the website | Future |
