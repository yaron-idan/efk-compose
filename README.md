# efk-compose
Just run `docker-compose up --build`
When all services are up, run `curl localhost:8080`
You can then query your logs in one of two ways -
1. Access `localhost:5601` in your browser, and query the log sent from fluentd to ES.
2. Query ES directly from the command line like so - `curl 'localhost:5601/fluentd-<YYYYMMDD>/_search?pretty'`
