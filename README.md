# helm-openshift 


helm upgrade  esign  ./ipos   \
--install \
--wait \
--debug \
--timeout 50m0s \
--namespace   \
--set metadata.namespace= \
--set image.tag= \
--set image.registry= \
--set image.repository= \
--set ingress.hosts[0].host= \
--set ingress.hosts[0].paths[0].path=/ \
--set ingress.hosts[0].paths[0].pathType=Prefix \
--set volume.volumes.csi.volumeAttributes.secretProviderClass=  \
--set AzureIdentity.spec.resourceID=   \
--set AzureIdentity.spec.clientID=  \
--set AzureIdentity.AzureIdentityBinding.name=  \
--set SecretProviderClass.secret.objects.objectName=    \
--set SecretProviderClass.parameters.keyvaultName=  \
--set SecretProviderClass.parameters.userAssignedIdentityID=  \
--set SecretProviderClass.parameters.tenantId= 



