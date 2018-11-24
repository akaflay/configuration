# configuration

This is just a git repo where we can add all the different properties for different Micro services. These properties can be pulled by the config server
and provided to the required microservice. The file pulled is based on the name of the application.

e.g If the value of spring.application.name=app in the application properties of the application. The config file from this repo with name 
app.properties, app.yml and aplication.properties will be returned. Below is an exemple response

## Exemple

```
{
    "name": "app",
    "profiles": [
        "default"
    ],
    "label": null,
    "version": "2cc799b460b4df6ed8b7a4d9be310eec84ae6200",
    "state": null,
    "propertySources": [
        {
            "name": "https://github.com/akaflay/configuration//app.properties",
            "source": {
                "server.port": "8082"
            }
        },
        {
            "name": "https://github.com/akaflay/configuration//app.yml",
            "source": {
                "server.port": 8082
            }
        },
        {
            "name": "https://github.com/akaflay/configuration//application.properties",
            "source": {
                "server.port": "8081"
            }
        }
    ]
}
```
