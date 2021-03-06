proteus-aws-operator
====================

The Proteus AWS Operator is used to extend the functionality of AWS Controllers for Kubernetes (ACK).

Currently supported CustomResourceDefinitions (and related controllers)
-----------------------------------------------------------------------

1. DBReplicationGroup

    Used to create multiple DBInstance instances (NumReplicas in each AvailabilityZone) using the ACK RDS Controller.

Requirements
------------

1. Operator SDK

	https://sdk.operatorframework.io/docs/installation/


Testing
-------

To run the tests:

	make test


Building
--------
To build the Docker image and create the deployment yaml files

	make docker-build docker-push IMG="docker-proteus-aws-operator-test.dr-uw2.adobeitc.com/proteus-aws-operator:v0.0.1"

Notes
-----

1. Testing docker repository: `docker-proteus-aws-operator-test.dr-uw2.adobeitc.com`
