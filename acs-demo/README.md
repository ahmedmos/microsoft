# Documentation for the Azure Container Service Demo

In the Azure Container Service Demo I demo the following
 * Create an ACS environment, use the source 01-createAcsDcos.sh
   * I start with this because it takes time to create the acs environemnt..during the create I will show docker basics
   * Show how you can start this script from a CD pipeline with jenkins as example
 * Docker, start a local twitterapp using the sources in acs-demo/twitterapp 
   * a lightweight springboot app, explain about the dockerfile
   * go into the dockerfile, commit, volumes, tag en submit to repository
 * Docker Compose, using the sources in acs-demo/java-webapp-redisdemo
   * explain about relationship between containers with link 
   * docker-compose up
 * Now Explain about complexity of containers in productionlandscape --> container orchestation required 
   * bringing the java-webapp-redisdemo to production with mesos
     * load the marathon-lb
     * redis.json, explain about persistancy and this (non clustered solution) about linking with labels and healthcheck
     * java-webapp-redisdemo.json