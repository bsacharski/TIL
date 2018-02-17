## Services

### Services naming convention
Never EVER name your service in a generic way.
Kubernetes creates an env variables based on service names.
For instance, service `FOO` with some port exposed will cause k8s to generate
`FOO_PORT` variable (among many others).
You can probably see what happens if you name your service `Redis`.
