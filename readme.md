# app-advisor-demo-spring-petclinic

This is a sample repo to demo Spring Application Advisor capabilities.
This specific repo is the copy of [spring-petclinic](https://github.com/pivotal-cf/spring-petclinic/tree/2.7.3-demo).
Please check the latest [spring-petclinic](https://github.com/spring-projects/spring-petclinic).

Read the original [readme.md](readme-original.md)

## Spring Application Advisor

See [Spring Application Advisor Documentation](https://docs.vmware.com/en/Tanzu-Spring-Runtime/Commercial/Tanzu-Spring-Runtime/index-app-advisor.html) for details.

## Get Started

* [Fork this project first](https://github.com/nevenc/app-advisor-demo-spring-petclinic/fork), e.g.

```
git clone git@github.com:YOUR_NAME_HERE/app-advisor-demo-spring-petclinic.git
```

* Open the project, e.g. 

```
cd app-advisor-demo-spring-petclinic
```


## Run the Advisor CLI

* Run the Advisor to get a build configuration, e.g.

```
advisor build-config get
```

* Get the Upgrade Plan, e.g. 

```
advisor upgrade-plan get 
```

* Apply the Upgrade Plan step, e.g.

```
advisor upgrade-plan apply 
```

* Alternatively, do a pull request as well. Make sure you have configured Github token (classic) for automated pull requests, e.g.

```
export GIT_TOKEN_FOR_PRS=<YOUR_GIT_TOKEN_FOR_PULL_REQUESTS>
advisor upgrade-plan apply --push
```

## Rinse and repeat

* Review, and test the pull requests.

* Merge once you are comfortable with the changes.

* Rinse and repeat until you are at the latest available release, e.g. 

```
git restore .
git pull
advisor build-config get
advisor upgrade-plan get 
advisor upgrade-plan apply --push
```
