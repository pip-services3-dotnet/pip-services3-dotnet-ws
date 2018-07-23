# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for Pip.Services in .NET

This is a workspace for [Pip.Services](https://github.com/pip-services/pip-services) frameworks implemented in .NET. 
It enables build, test, and release across the following projects:

- **pip-services-devenv** - dockerized infrastructure services for development and testing
- **pip-services-commons-node** - basic portable abstractions
- **pip-services-components-node** - component definitions
- **pip-services-test-node** - component definitions
- **pip-services-container-node** - IoC containers
- **pip-services-data-node** - Data processing and persistence components
- **pip-services-rpc-node** - remote procedure calls
- **pip-services-messaging-node** - asynchronous messaging
- **pip-services-elasticsearch-node** - ElasticSearch components
- **pip-services-fluentd-node** - Fluentd components
- **pip-services-memcached-node** - Memcached components
- **pip-services-redis-node** - Redis components
- **pip-services-mongodb-node** - MongoDB components
- **pip-services-prometheus-node** - Prometheus components
- **pip-services-aws-node** - AWS components
- **pip-services-azure-node** - Azure components
- **pip-services-echo-node** - sample echo microservice

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-dotnet-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services/pip-services-dotnet-ws.git
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
> piptask start -component pip-services-devenv
> piptask stop -component pip-services-devenv
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
