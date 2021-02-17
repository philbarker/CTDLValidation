# CTDLValidation
Config files and SHACL shape definitions for validating CTDL instances using a local installation of the EC ISA ITB [SHACL RDF Validator](https://www.itb.ec.europa.eu/shacl/any/upload). SHACL shapes are provided for the Credential Engine Registry required and minimal benchmark profiles as described in the Credential Engine Registry [Minimum Data and Currency Policy](https://credreg.com/registry/policy).

[A guide](https://www.itb.ec.europa.eu/docs/guides/latest/validatingRDF/index.html) for setting up a local installation of the ITB RDF Validator (and other parts of the testbed) is available on the GITB website.

The SHACL shapes should be useful for other SHACL-based RDF validators.

## Directory Structure
```
CTDLValidation
.
├── README.md
├── samples (valid and invalid instance data)
│   ├── comptency_req_4errors.ttl
│   ├── comptency_req.ttl
│   ├── credOrg_rec_valid.ttl
│   ├── credOrg_rec_warnings.ttl
│   ├── credOrg_req_5errors.ttl
│   ├── credOrg_req_valid.ttl
│   ├── NCCER_errors.json
│   └── no-nodes.ttl
└── validator
    ├── Dockerfile (Docker config file for isaitb/shacl-validator)
    └── resources
        ├── Competency
        │   ├── config.properties (validator config for Competency shapes)
        │   └── shapes
        │       ├── comp_rec.ttl
        │       └── comp_req.ttl
        ├── CredentialOrganization
        │   ├── config.properties
        │   └── shapes
        │       ├── credOrg_rec.ttl (to be done)
        │       └── credOrg_req.ttl
        └── QAOrganization

```
