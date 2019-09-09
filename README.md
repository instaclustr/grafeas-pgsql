
# grafeas-pgsql

  

This is a fork of [Grafeas](https://github.com/grafeas/grafeas) with a PostgreSQL backend specified in the configuration file, provides a standalone instance of the Grafeas server with PostgreSQL as the storage layer. The postgresSQL url should be changed to your storage instance with credentials updated.

  

## Running Standalone Grafeas with PostgreSQL

  

To start the standalone instance of Grafeas with PostgreSQL, follow these steps:

  

1. Pull the Grafeas Server image:

  

```bash

docker pull us.gcr.io/grafeas/grafeas-server:0.1.0

```

  

2. Build the images 

  

```bash

docker build -f docker/Dockerfile -t grafeas_pgsql .

```

  

3. Run the docker image:

  

```bash

docker run -p 8080:8080 -v config.yaml:/config.yaml grafeas_pgsql

```

  

4. Ensure you can reach the server:

  

```bash

curl http://localhost:8080/v1beta1/projects

```

  

## Contributing

  

Pull requests and feature requests as GH issues are welcome!

  

## License

Grafeas is under the Apache 2.0 license. See the [LICENSE](LICENSE) file for details.
