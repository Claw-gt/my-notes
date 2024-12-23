
```mermaid
flowchart TD
RootCA --- IssuingCA_1
RootCA --- IssuingCA_2
IssuingCA_1 --- EndEntity_Certificates_1
IssuingCA_2 --- EndEntity_Certificates_2
```

Direct registration is prevented through **Registration Authorities (RAs)**

```mermaid
flowchart TD
RootCA --- IssuingCA_1
RootCA --- IssuingCA_2
IssuingCA_1 --- RA_1
IssuingCA_2 --- RA_2
RA_1 --- LRA_1.0
RA_1 --- LRA_1.1
LRA_1.0 --- EndEntity_Certificates_1
RA_2 --- LRA_2.0
RA_2 --- LRA_2.1
LRA_2.0 --- EndEntity_Certificates_2
```



Siemens Maufacturer: **Root CA** ------- offline
-
Manufacturer: **Issuing CA                 Signer: **Issuing CA**  -------------  Siemens Trust Center
-
Siemens Mobility Manufacturing Facilitites: **LRA** --> acts as a proxy in front of the manufacturer Issuing CA to prevent the enrollment of certificates for non existing fake devices


