# CAPS

> An attempt to mitigate resource exhaustion using cgroups features directly in compose.yaml for Docker containers

> [!TIP]
> Don't let technical problems KILL your AMBITIONS...

![visitor badge](https://visitor-badge.laobi.icu/badge?page_id=alexandreelise.caps&style=flat&format=true)
![GitHub followers](https://img.shields.io/github/followers/alexandreelise?style=flat)
![YouTube Channel Views](https://img.shields.io/youtube/channel/views/UCCya8rIL-PVHm8Mt4QPW-xw?style=flat&label=YouTube%20%40ApiAdept%20vues)


## PRE-REQUISITE:

- Know how to use the command line
- Know docker and docker compose basic commands 


## USAGE:

3 steps :

Step 1:

Clone this repo or use the example ```compose.yaml``` file and adapt it:

```shell

git clone https://github.com/alexandreelise/caps

```

Step 2:

Go to the directory you just cloned and run that command in your terminal

```shell

cd caps &&
APP_IMAGE=php:8.5-apache  docker compose up -d

```

or 

```shell

cd caps &&
APP_IMAGE=replace_with_your_favourite_docker_image_here  docker compose up -d

```

Step 3:

Run ```shell docker compose stats ``` command to **VERIFY** the **RESOURCES** are **ACTUALLY** **RESTRICTED** as **EXPECTED**

```shell

docker compose stats

```

That's it! You have successfully mitigated resource exhaustion of your system.


