# What's new in ibm-sam v1.2.0 Chart
This chart is based on the original v1.0.0 Chart (published in ICP repo) with the following changes:
* The ability to add an OpenLDAP deployment to the release
* The ability to specify a pre-created secret for key material for OpenLDAP and PostgreSQL deployments
* The ability to specify instance names for Reverse Proxy instances
* Update to use 9.0.7.1_IF4 image tag (required for snapshot failure issue)
* Update to use ibmcom/isam repository (image will no longer be in store)
* Update ibm-sch to 1.2.15 required to support Helm 3.x.
* Support for Interim Fix images.
    * The tag parameter (which was appended to all repositories) is removed
    * Ability to specify the tag as part of the repository dbrepository and ldaprepository parameters instead.
* Update to use ReadWriteOnce disks and, to support this, use separate PVCs for different containers.
* Lower minimum memory and CPU requirements to allow deployment in dev/test environments

# Documentation (for original IBM Security Access Manager Charts)
For detailed documentation instructions go to [https://www.ibm.com/support/knowledgecenter/en/SSPREK/welcome.html](https://www.ibm.com/support/knowledgecenter/en/SSPREK/welcome.html).


# Version History

| Chart | Date | Kubernetes Required | Image(s) Supported | Breaking Changes | Details
| ----- | ---- | ------------------- | ------------------ | ---------------- | -------
| 1.2.0 | April 2020  | >= 1.11.x | ibmcom/isam:9.0.7.1_IF4; ibmcom/isam-postgresql:9.0.7.0; ibmcom/isam-openldap:9.0.7.0 | docker hub | Based on original v1.0.0 chart
