+++
title = "Setting up Cloud9 IDE"
weight = 200
+++

#### Navigate to Cloud9 section

![](./9.png)

----

#### Create Cloud9 environment

![](./10.png)

----

![](./11.png)

----

#### Configure your Cloud9 environment

![](./12.png)

----

#### Select **Network (VPC)** from **Network settings**

![](./18.png)

----

#### Review and create

![](./13.png)

----

#### Wait for IDE to be ready

![](./14.png)

----

{{% notice info %}}
If you see this Error message, click `OK` to proceed 
{{% /notice %}}

![](./17.png)

----

From a terminal window, run:

```
aws sts get-caller-identity
```

Verify if `assumed role` shows as below

```
arn:aws:sts::YOUR_AWS_ACCOUNT_ID:assumed-role/TeamRole/MasterKey
```


To check CDK version, run:

```
cdk --version
```

Verify if version is `1.110.` or **higher**

![](./19.png)

## Now let's upgrade CDK to its latest version

```
npm install -g aws-cdk --force
```

----


#### Troubleshooting

{{% notice warning %}}
If you get logged out of AWS Console, try following steps to obtain new `temporary credentials`
{{% /notice %}}

![](./15.png)

![](./16.png)

![](./20.png)