# EMLO Session 10

The objective of this session was to implement CI/CD on AWS using CodeCommit, CodeBuild, and CodeDeploy.


# Task 1

We are required to add an artifact. 

The following lines were added to `buildspec.yml`

```
artifacts:
  type: zip
  paths:
    - './build/**/*'
```

After the build successfully completes,  we can see the log

![](./img/build_success.png)

We can also see our artifact created.

![](./img/artifact_res.png)


Auto-build using cloudwatch also works fine

![](./img/autobuild_success.png)


We can also see the result of our site

![](./img/web_after_autobuild.png)

# Task 2
We are required to change the code and implement CodeDeploy. This has been done successfully.


![](./img/deploy.png)

Running the curl command gives the following results.

![](./img/final.png)
