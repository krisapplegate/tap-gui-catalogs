# Spring PetClinic Example

This is an example of the [Spring PetClinic](https://github.com/spring-petclinic/spring-framework-petclinic)
server deployed as a [CNR](https://docs.vmware.com/en/Cloud-Native-Runtimes-for-VMware-Tanzu/1.0/tanzu-cloud-native-runtimes-1-0/GUID-cnr-overview.html)
service.

## Deploy Petclinic with kapp

Simply run:

```
kapp deploy -a petclinic -f k8s.yml
```

This will create a namespace called `petclinic`, a mysql Deployment and a Knative service
running petclinic.

## Backstage catalog

A very basic catalog is provided in the `catalog` folder. You can add it to your backstage
by referencing it from gitlab
