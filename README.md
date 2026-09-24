# iServerSupport Cloud Server Provisioning

A Crossplane Configuration package for provisioning AWS cloud servers through
a simple composite resource API.

## What it provides

The package defines:

- `CloudServer` claim
- `XCloudServer` composite resource
- AWS EC2 instance Composition
- Pipeline-based Patch & Transform composition
- Configurable AWS region
- Configurable EC2 instance type
- Configurable AMI
- Configurable AWS ProviderConfig

## Example

```yaml
apiVersion: compute.iserversupport.com/v1alpha1
kind: CloudServer
metadata:
  name: example-server
spec:
  region: us-east-1
  instanceType: t3.micro
  ami: ami-0123456789abcdef0
  providerConfigRef: default

The package requires the Upbound AWS EC2 provider and the Crossplane
Function Patch & Transform.

Package

Configuration package:

iServerSupport Cloud Server Provisioning

Cloud Server Management

For cloud server management, Linux server administration, monitoring,
security, and infrastructure support:

https://iserversupport.com/cloud-server-management/
