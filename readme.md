
mvn clean deploy - for version update for example 1.0.0 to 1.0.1
//Sandbox env - for build and re-redeploying
mvn -DmuleDeploy deploy -DskipTests -Dap.client_id=227ad54ef64941b9b7602e6e92a9c753 -Dap.client_secret=2BCf8081134444b8896b42485bCd3148 -Dap.ca.client_id=1bab1f0b3c8a45ea9e39d33bd56bbb1f -Dap.ca.client_secret=C382306D1CF946Db9571E1707BA703f8 -Dencrypt.key=dev-lewisccx-poc -Ddeployment.env=Sandbox -Dapi.env=sit -Dap.target=Cloudhub-US-East-2 -Dap.vcore=0.1 -Dap.replica=1 -Dmule.artifact=target/poc-prototype-api-1.0.32-mule-application.jar -Dap.mule.version=4.6.20 

keystore password: dev-lewisccx-poc