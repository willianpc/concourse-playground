# concourse-playground
Playing with concourse ci

### Start Concourse

    $ docker-compose up

Concourse will run under ``http://localhost:8080/``

User/password is test/test


### Running tests with dynamic data from ytt

    $ ytt -f go-sensor-ytt.yml -f ytt-data.yml | fly -t tutorial set-pipeline -p my-pipeline -c -