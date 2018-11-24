# Configurations

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
    "version": "09be70d0cf3d0eea54990b8e3eab6e13d4e2d10f",
    "state": null,
    "propertySources": [
        {
            "name": "https://github.com/akaflay/configuration//app.properties",
            "source": {
                "db.url": "jdbc:mysql://127.0.0.1/college",
                "db.user": "root",
                "db.password": "root"
            }
        },
        {
            "name": "https://github.com/akaflay/configuration//app.yml",
            "source": {
                "db.url": "jdbc:mysql://127.0.0.1/college",
                "db.user": "root",
                "db.password": "rootroot"
            }
        },
        {
            "name": "https://github.com/akaflay/configuration//application.properties",
            "source": {
                "db.url": "jdbc:mysql://127.0.0.1/college",
                "db.user": "root",
                "db.password": "rootroot"
            }
        }
    ]
}
```

## Questions and Concerns
https://better-coder.slack.com/
