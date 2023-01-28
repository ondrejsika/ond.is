# [ond.is](https://ond.is)

    Ondrej Sika <ondrej@ondrejsika.com>
    https://github.com/ondrejsika/ond.is

My Icelandic site.

## Build, Push & Deploy

```
docker build --platform linux/amd64 -t ondrejsika/ond.is .
docker push ondrejsika/ond.is
helm repo add ondrejsika https://helm.oxs.cz
helm upgrade --install ond-is ondrejsika/one-image --set host=ond.is --set image=ondrejsika/ond.is
```
