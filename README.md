# PCF Get Environment Variables
Simple GO app that will display the environment variables for a given application name.

## Required Environment Variables for a PCF Deploy
If you are deploying this into PCF, you must provide the following environment variables.

* `application_name` => Default PCF config value, used by the application so that any request for the environment variables of a know admin tool (with admin credentials) doesn't return any values
* `SKIP_SSL_VALIDATION` => Set to `true` when using self-signed certs
* `API_ADDRESS` => Set to the API endpoint - typically `https://api.<systemDomain>`
* `API_USERNAME` => Set to an API admin, typically `admin`
* `API_PASSWORD` => Set to the password for the given `API_USERNAME`
* `PORT` => Port the app should run on

### Clone and run
The project uses [Glide](https://github.com/Masterminds/glide) to manage dependencies.

To get started, simply clone the project, and run `glide install`.  You should then be able to run `go run main.go`

# Issues
Please use the [Issues tab](../../issues) to report any problems or feature requests.
