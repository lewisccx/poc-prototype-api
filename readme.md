
mvn clean deploy - for version update for example 1.0.0 to 1.0.1
//Sandbox env - for build and re-redeploying

mvn clean validate
mvn clean -DmuleDeploy -DskipTests deploy -P Windows,CloudHub2 -Dap.businessGroupId=43741aa3-8578-46e7-ba11-bec80c101db9 /
	-Dap.clientId=b9a13cfb38044161a52076ff9afba915 /
	-Dap.clientSecret=C63BBD0e324c4fe2A04F376b7a716c5F /
	-Dap.ca.client_id=9c5622cde38b41b9bccc78cb45a2f7cb /
	-Dap.ca.client_secret=41Cb7D686b864e7884D1547b68870c17 /
	-Ddeployment.env=SIT -Dapi.env=sit /
	-Dap.target=Cloudhub-US-East-2 /
	-Dap.vCores=0.1 -Dap.replicas=1 /
	-Dap.deploymentTimeout=600000 /
	-Dap.skipDeploymentVerification=false / 
	-Dap.objectStoreV2=true /
	-Dap.updateStrategy=rolling / 
	-Dap.visualizerLayer /
	-Dap.enableMonitoring=true -Dap.mule.version=4.9.16

mvn -DmuleDeploy deploy -DskipTests -Dap.client_id=227ad54ef64941b9b7602e6e92a9c753 

-Dap.client_secret=2BCf8081134444b8896b42485bCd3148 -Dap.ca.client_id=1bab1f0b3c8a45ea9e39d33bd56bbb1f -Dap.ca.client_secret=C382306D1CF946Db9571E1707BA703f8 -Dencrypt.key=dev-lewisccx-poc -Ddeployment.env=Sandbox -Dapi.env=sit -Dap.target=Cloudhub-US-East-2 -Dap.vcore=0.1 -Dap.replica=1 -Dmule.artifact=target/poc-prototype-api-1.0.32-mule-application.jar -Dap.mule.version=4.9.16 

keystore password: dev-lewisccx-poc