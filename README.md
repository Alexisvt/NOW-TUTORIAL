# Now Lesson Resume

## How to install **Now**

```cmd
npm i -g now
```

## How to deploy a docker container or a node app

```cmd
c:\MyAppOrDockerContainerFolder> now
```

## How to force to deploy something staticly

```cmd
c:\MyApp> now --static
```

## How to alias a deploy url

```cmd
now alias my-last-deploy-url.now.sh new-alias
```

Where new-alias is the new **alias** for the desire deploy url

## Special package.json keys

* `now-start`: replace `start` package command
* `now-build`: replace `build` package command

## How to make a deployment *public*

```cmd
now -p 
```

## How to change our code live in now

* First we need to go the url that we deploy
* Then We need to append to the url `_src` and hit enter

Sample:

http://my-last-deploy-url.now.sh/_src 

Everytime that we highlight something It will generate a url that we can share with others to point the error

## How to configure an environment variable with **Now**

```cmd
c:\MyApp> now -e KEY=VALUE
```

and if we want to set multiple variables:

```cmd
c:\MyApp> now -e KEY1=VALUE1 -e KEY2=VALUE2
```

## How to define a secret with **Now**

First we need to set our secrets

```cmd
c:\MyApp> now secret add variableName VALUE
```

Now to call that variableName's value:

```cmd
c:\MyApp> now -e KEY=@variableName
```

To show the documentation about the `secrets`

```cmd
c:\MyApp> now secrets
```

## How to show all the secrets in our account

```cmd
c:\MyApp> now secrets ls
```

## How to remove an specific secret

```cmd
c:\MyApp> now secret remove secretName
```

## How to 