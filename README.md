# WORDPRESS I OPENSHIFT
## INFO 
Vi hjälper Firman AB att bygga och deploya WordPress i ett OpenShift-kluster. Målet med uppgiften var att sätta upp en lösning där WordPress är tillgänglig via en webbadress (http://…) och att webbplatsen fortsätter fungera även om poddar startas om.
## BESKRIVNINGAR
-- 01_storage.yaml
definierar pvc för wordpress och mysql-databas  
```bash
oc apply -f 01_storage.yaml  
-- 02_mysql.yaml  
definierar deployment och service för databasen  
```bash
oc apply -f 02_mysql.yaml

