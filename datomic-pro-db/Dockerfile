FROM datomic-pro-base

ARG DATOMIC_LICENSE_KEY
ENV MY_DATOMIC_LICENSE_KEY $DATOMIC_LICENSE_KEY

# run with this CMD format in order for the MY_DATOMIC_LICENSE_KEY environment variable to surface
CMD transactor -Ddatomic.licenseKey=${MY_DATOMIC_LICENSE_KEY} config/dev-transactor.properties

EXPOSE 4334 4335 4336
