# simplest-springboot-app

##deploy on opensihft
- prerquisite
  - An openshift cluster is running
- open console 
  - Create a project
  - Go to developer perspective -> Add+
  - select 'From Git'. Provide git url for this project and hit 'Create'
- Access the app on browser http:// < route > /welcome/message
  
## deploy via cli
  - oc new-project < project name >
  - oc new-app java~https://github.com/IndraniDey1/simplest-spring-boot-app.git
  - oc expose svc/simplest-spring-boot-app
  - oc get route
  - Access app : http:// < route > /welcome/message
