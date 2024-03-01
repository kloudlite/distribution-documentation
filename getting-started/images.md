# Images

Kloudlite allow you to push your images inside your container repository.

Please follow below steps to push your images.

Open your terminal and execute the following command:

* ### Login using credentials

```
# login
docker login

# provide username and password
- dashboard > packages > access management
- <copy username and password from container registry list>
```

* ### Tag Image

```
# Tag image
docker tag <image_name>:<image_tag> <containerrepo_url>:<image_tag>
eg: docker tag httpd:latest registry.dev.kloudlite.io/demo-team/demo_repo:main
```

* ### Push Image

```
# Push Image
docker push <containerrepo_url>:<image_tag>
eg: docker push registry.dev.kloudlite.io/demo-team/demo_repo:main
```

* ### Pushed Images

```
# Steps to see pushed images
dashboard > packages > container repos > select repo > images
```

<figure><img src="../.gitbook/assets/Screenshot 2024-03-01 at 5.24.59 PM.png" alt=""><figcaption></figcaption></figure>
