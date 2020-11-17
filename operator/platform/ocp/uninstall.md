# Uninstalling IBM Content Collector for SAP ga-4.0.0.4 on Red Hat OpenShift

## Delete the Operator

To uninstall the deployments and the Content Collector for SAP operator, use the 'deleteOperator.sh' command to delete all the resources that are linked to the operator.

```bash
   ./scripts/deleteOperator.sh
```

Verify that all pods created with the deployment are terminated and deleted.

## Delete deployments

If you want to delete the custom resource deployment, you can delete the corresponding YAML file.

For example:
```bash
  $ oc delete -f descriptors/my_iccsap_v1_iccsap_cr.yaml
```

To uninstall an instance of the operator, you must delete all of the manifest files in the cluster:

```bash
  $ oc delete -f descriptors/operator.yaml
  $ oc delete -f descriptors/role_binding.yaml
  $ oc delete -f descriptors/role.yaml
  $ oc delete -f descriptors/service_account.yaml
  $ oc delete -f descriptors/iccsap_v1_iccsap_crd.yaml
```


