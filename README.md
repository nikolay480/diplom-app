
https://cloud.yandex.ru/docs/container-registry/operations/authentication#sa


# Аутентификация с помощью OAuth-токена
`$ docker login --username oauth --password `

```bash

y0_AgAAAABlxVV0AATuwQAAAADT2IR01JfYAAbMTr-6_qc2eFMMWEu2T-Y cr.yandex
WARNING! Using --password via the CLI is insecure. Use --password-stdin.
WARNING! Your password will be stored unencrypted in /home/nik/.docker/config.json.
Configure a credential helper to remove this warning. See
https://docs.docker.com/engine/reference/commandline/login/#credentials-store

Login Succeeded

```

```bash
$ cat key.json | docker login \
  --username json_key \
  --password-stdin \
  cr.yandex
WARNING! Your password will be stored unencrypted in /home/nik/.docker/config.json.
Configure a credential helper to remove this warning. See
https://docs.docker.com/engine/reference/commandline/login/#credentials-store

Login Succeeded
```
