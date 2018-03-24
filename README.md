# gcp-metadata

Script for getting the gcp instance informations. 
It is very similar to aws-metadata (https://aws.amazon.com/code/ec2-instance-metadata-query-tool/)

For more information on Google Cloud meta-data, refer to the documentation at
https://cloud.google.com/compute/docs/storing-retrieving-metadata

## Prerequisites
1. Linux Environment running on GCP
2. curl package

## Usage
```
    gcp-metadata v1.0.0

    Use to retrieve GCP instance metadata from within a running GCP instance.
    e.g. to get instance id: 'gcp-metadata -i'
		 to get instance type: 'gcp-metadata -t'
		 to get help: 'gcp-metadata --help'

    For more information on Google Cloud meta-data, refer to the documentation at
    https://cloud.google.com/compute/docs/storing-retrieving-metadata

    Usage: gcp-metadata <option>

    Options:
    --h/--help                  Show help on the command
    --all                       Show all metadata information
    -p/--project-id             The Project, the instance belongs to.
    -a/--image                  Image of the instance (Currently not available)
    -n/--instance-name          Name of the instance as it appears on the GCP Console
    -i/--instance-id            Numeric instance-id of the instance
    -t/--instance-type          The type of instance. Details @ https://cloud.google.com/compute/docs/machine-types
    -h/--local-hostname         The local hostname of the instance.
    -o/--local-ipv4             Private IP of the instance
    -v/--public-ipv4            NATted Public IP of the instance
    -m/--mac                    MAC Id of the instance
    -z/--availability-zone      The availability zone in which the instance is launched.
    -e/--description            Description of the instance
    -d/--disks                  All the disks attached to the instance
    -s/--service-account        IAM Profile / Service Account attached to the instance
    -l/--instance-template      Instance template used to launch the instance
    -c/--created-by             Source that created the instance, like instance group
    -g/--tags                   Tags associated to the instance
    -u/--user-data              User-supplied data. Available only if it is supplied at instance launch time.
```

