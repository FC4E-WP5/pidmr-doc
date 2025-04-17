---
id: pidmr_parser
title: PIDMR Parser
sidebar_position: 5
---

### Step-by-Step Guide parse the result of the PIDMR 

PIDMR resolver parser service is a small library that was created during the project in node.js
The PIDMR parser gets as input a PID, makes a request to PIDMR service, and given the response parses it to a json object.
if there is a parser available for the given endpoint.

#### Example 

Example Request:

```
curl http://pidmr-service-url/10.5524%2F100005
```
The result that is created is of the following format 

```json

{"id":"10.5524/100005","type":"dataset","title":"Genomic data from the Emperor penguin (Aptenodytes forsteri)","result":{"accessRights":"OPEN","embargoEndDate":"","authors":["Li, J","Zhang, G","Lambert, D","Wang, J"],"editors":[],"source":"datacite","publisher":"GigaScience","journal":null,"DOI":"10.5524/100005","url":"https://doi.org/10.5524/100005","date":2011}}

```

You may find the code and more details from [here](https://code-repo.d4science.org/argiro.kokogiannaki)
