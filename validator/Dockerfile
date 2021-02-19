FROM isaitb/shacl-validator:latest
COPY resources /validator/resources/
ENV validator.resourceRoot /validator/resources/
ENV validator.domain CredentialOrganization, Competency
# the following are currently set low (100s) for development purposes
ENV validator.cleanupRate 100000
ENV validator.cleanupWebRate 100000
