# SNOW-IntegrationHUB
Practical
- Inactivate business rules from webservices demo and inactivate  flow demos
- Enable plugins
- Activated ServiceNow IntegrationHub Installer
- Activated ServiceNow IntegrationHub Standard Pack Installer

## target instance 
- user itil and rest_service roles
- instance url

## source instance 
### IntegrationHub
1.	Credentials (get from target user id and url)
2.	connect
3.	Action designer opens flow designer to trigger

### credentials->new basic auth credentials 
-	give name 
-- credentials->new basic auth credentials
-- give name
-- give user name from the target instance + pw 
-	give user name from the target instance + pw 
-	save

### connections-> new
-	http(s) connection give name
-	creds you just created 
-	connection alias sn_ebonding_ah.ServiceNow
-	connection url: target instance URL 
-	make sure url has https:// and no / or whitespaces at the end >.> 

### create flow designer 
-	new
-	name: training integration hub
-	add trigger -> created incident table
-	add condition like category ABC ect 
-	add actions->action->servicenow ebonding create remote incident click on datapill trigger incident record
-	save
-	activate
-	test
-	Deactivate workflow


![image](https://user-images.githubusercontent.com/12488769/147857937-d9e8680a-95f0-4b09-a868-11ae973b136e.png)
![image](https://user-images.githubusercontent.com/12488769/147857973-4ed7d65f-879f-4f36-9fa7-bdae60b0d23d.png)

