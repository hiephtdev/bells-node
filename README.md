# How to Run a Bell Node with Docker Compose

This guide will walk you through running a Bell Node using Docker Compose. Make sure you have Docker and Docker Compose installed before getting started.

## Step 1: Clone the Source Code

Clone the source code of Bell Coin Core from the [official repository](https://github.com/bellscoin-community/bellscoinv2) and create a configuration file `bells.conf` as per your requirements.

## Step 2: Pull a docker-compose.yml File

Pull a `docker-compose.yml` file in repo:

```bash
git clone https://github.com/hiephtdev/bells-node
cd bells-node
```

## Step 3: Run the Bell Node

Open a terminal and navigate to the directory containing the docker-compose.yml file. Then, run the following command to start the Bell Node:

```bash
docker-compose up -d
```

This will create and start the Bell Node container.

## Step 4: Check the Status of the Bell Node

To check the status of the Bell Node, you can use the following command:

```bash
docker logs -f bell-node-ct
```

This command will display the container's logs, allowing you to monitor the synchronization process and the operation of the Bell Node.

## Step 5: Stop the Bell Node (if needed)

If you want to stop the Bell Node, you can use the following command:

```bash
docker-compose down
```

This will stop and remove the Bell Node container, but your data and configuration will be stored in volumes.

Congratulations! You have successfully run a Bell Node using Docker Compose. You can customize the bells.conf configuration file to suit your needs.

## Contributing and Support

If you encounter issues or want to contribute to this project, please create an issue or pull request on the [GitHub repository](https://github.com/hiephtdev/bells-node). We welcome your contributions.
