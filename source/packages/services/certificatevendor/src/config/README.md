## The following mandatory env config needs defining per environment:

```ini
ASSETLIBRARY_API_FUNCTION_NAME=
AWS_IOT_ENDPOINT=
AWS_REGION=
AWS_S3_CERTIFICATES_BUCKET=
CERTIFICATES_CACERTIFICATEID=
POLICIES_ROTATEDCERTIFICATEPOLICY=
```

## The following may be overridden:

```ini
AWS_IOT_THINGGROUP_ROTATECERTIFICATES=cdfRotateCertificates
AWS_S3_CERTIFICATES_PREFIX=certificates/
AWS_S3_CERTIFICATES_SUFFIX=.zip
AWS_S3_CERTIFICATES_PRESIGNEDURL_EXPIRESINSECONDS=300

MQTT_TOPICS_GET_SUCCESS=cdf/certificates/{thingName}/get/accepted
MQTT_TOPICS_GET_FAILURE=cdf/certificates/{thingName}/get/rejected
MQTT_TOPICS_GET_ROOT=cdf/certificates/+/get
MQTT_TOPICS_ACK_SUCCESS=cdf/certificates/{thingName}/ack/accepted
MQTT_TOPICS_ACK_FAILURE=cdf/certificates/{thingName}/ack/rejected
MQTT_TOPICS_ACK_ROOT=cdf/certificates/+/ack

FEATURES_DELETEPREVIOUSCERTIFICATE=false

DEFAULTS_DEVICE_STATUS_SUCCESS_KEY=status
DEFAULTS_DEVICE_STATUS_SUCCESS_VALUE=active
DEFAULTS_CERTIFICATES_CERTIFICATEEXPIRYDAYS=1095

REGISTRY_MODE=Assetlibrary

LOGGING_LEVEL=info
```