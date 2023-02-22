# testcontainer-postgres
## Prerequisite
1. Testkube helm chart is already installed in the cluster
2. Testkube CLI

## Create Test
For creating the test, we will be using gingko executor, run the below command
```
kubectl testkube create test --git-uri https://github.com/richamishra006/testcontainer-postgres.git --git-path ./ --type ginkgo/test --name postgres-test --git-branch master --git-username *** --git-token=***
```
git-uri- The github repo where the test code exists
git-path- The directory which needs to be referred for running the tests

Once we run the above command, test will be created
we can run the tests from UI, For accessing UI, run the below command:

```
kubectl testkube dashboard
```
