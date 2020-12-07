# <img src="https://uploads-ssl.webflow.com/5ea5d3315186cf5ec60c3ee4/5edf1c94ce4c859f2b188094_logo.svg" alt="Pip.Services Logo" width="200"> <br/> Workspace for .NET

This is a workspace for [Pip.Services V3](https://github.com/pip-services3/pip-services3) microservices toolkit implemented in .NET. It enables build, test, and release across the following projects:

- **pip-services3-devenv** - dockerized infrastructure services for development and testing
- **pip-services3-commons-node** - basic portable abstractions
- **pip-services3-components-node** - component definitions
- **pip-services3-test-node** - component definitions
- **pip-services3-container-node** - IoC containers
- **pip-services3-data-node** - Data processing and persistence components
- **pip-services3-rpc-node** - remote procedure calls
- **pip-services3-messaging-node** - asynchronous messaging
- **pip-services3-elasticsearch-node** - ElasticSearch components
- **pip-services3-fluentd-node** - Fluentd components
- **pip-services3-memcached-node** - Memcached components
- **pip-services3-redis-node** - Redis components
- **pip-services3-mongodb-node** - MongoDB components
- **pip-services3-prometheus-node** - Prometheus components
- **pip-services3-aws-node** - AWS components
- **pip-services3-azure-node** - Azure components
- **pip-services3-echo-node** - sample echo microservice

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-dotnet-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services3/pip-services3-dotnet-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop infrastructure services
```bash
> piptask start -component pip-services3-devenv
> piptask stop -component pip-services3-devenv
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The Node.js version of Pip.Services is created and maintained by:
- **Volodymyr Tkachenko**
- **Sergey Seroukhov**
- **Mark Zontak**
