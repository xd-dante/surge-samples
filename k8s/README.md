Chaos Testing
======================================

How to Run
-----------

1. Install and start minikube. Note: you'll need Docker too.

    ```sh
    minikube start --driver=virtualbox --memory=8192 # this can also work without virtualbox
    ```

   > Note: Before starting chaos testing please make sure you have compile and build [surge](https://github.com/UltimateSoftware/surge.git) reposiotry as this application depending on [surge](https://github.com/UltimateSoftware/surge.git) app so please compile surge before starting this test.

2. Start Chaos Testing

   This script perfoming following steps:

   - Building surge scala sample project
   - Installing Helm & Chaosblade
   - Starting Kafka using Streamzi
   - Starting Scala-Sample App in cluster
   - Starting Chaos Test cases
   - Gatling Test using scala

   ```sh
   Execute below script from k8s folder
   $ sh start-chaos-testing.sh
   ```

3. Clean Chaos Testing

   ```sh
   Execute below script to clean chaos testing 
   $ sh clean-chaos-testing.sh
   ```
