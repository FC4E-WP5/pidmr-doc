---
id: pidmr_backend
title: Metaresolver Backend
sidebar_position: 2
---

### Metaresolver Backend 

The Metaresolver is the main component that is responsible for the resolution of a PID and the presentation of a landing page, 
metadata or the underlying resource of the PID. A proxy server was set up based on the Handle Software which provides resolving 
service for the following PID providers in the current release:

 - Archival Resource Key (ARK PID) 
 - arXiv PID
 - SoftWare Hash persistent IDentifiers (SWHID)German urn:nbn PID (urn:nbn:de)
 - Finnish urn:nbn PID (urn:nbn:fi)
 - zenodo PID
 - Handles
 - DOIs

The proxy server of the Meta Resolver is available in a central point but resolving is possible via any handle resolving 
service using the handle PID 21.T11973/MR@ followed by the PID to be resolved. The service determines the structure 
of the information that can be expected from a resolution request and thus provides the possibility to request the landing page,
metadata or resource of the digital object specified via the PID. The resolver is able to recognize the PID type entered for 
resolution and knows where to route the request in order to get the requested information. 

The list of  PID providers is easily extendable so that a new PID can be onboarded without much effort. 
Performance testings based on determination of the dependency of the resolving performance on the number of providers were carried out 
which indicate no significant performance fluctuation. A detailed report about this is documented and can be reached under this [report](https://wiki.eduuni.fi/display/cscRDIcollaboration/Performance+Measurement+for+PIDMR). 

