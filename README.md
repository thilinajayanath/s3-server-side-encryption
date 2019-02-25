# check-s3-server-side-encryption

Simple script written in Python 3 that will check a given AWS account for the status of the default server-side encryption for all the S3 buckets and enable default server-side encryption with AES256.

## Prerequisites

These Python packages should be installed

```
boto3 - pip3 install boto3
botocore - pip3 install botocore
```

AWS named profile and credentials should be configured - [Read more](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html)

## Installation

* Clone the git repository
```
git clone git@github.com:thilinajayanath/check-s3-server-side-encryption.git
```

## Configuration

Replace the **AWS_PROFILE_NAME** in the following line with name of your profile for AWS credentials.

```
session = boto3.session.Session(profile_name='AWS_PROFILE_NAME')
```

## Run the application

```
chmod u+x enable_s3_encryption.py
./enable_s3_encryption.py
```

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details