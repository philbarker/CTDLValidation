FROM isaitb/shacl-validator:latest
COPY resources /validator/resources/
ENV validator.resourceRoot /validator/resources/
ENV validator.domain CredentialOrganization, Competency
# the following are currently set low (10s) for development purposes
ENV validator.cleanupRate 10000
ENV validator.cleanupWebRate 10000
