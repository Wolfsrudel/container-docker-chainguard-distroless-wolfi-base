# wolfi-base

<!---
Note: Do NOT edit directly, this file was generated using https://github.com/chainguard-images/readme-generator
-->

[![CI status](https://github.com/chainguard-images/wolfi-base/actions/workflows/release.yaml/badge.svg)](https://github.com/chainguard-images/wolfi-base/actions/workflows/release.yaml)

WORK IN PROGRESS

## Get It!

The image is available on `cgr.dev`:

```
docker pull cgr.dev/chainguard/wolfi-base:latest
```

## Supported tags

| Tag | Digest | Arch |
| --- | ------ | ---- |
| `latest` | `sha256:f580883564c381d3ff4c7af87c5779bb9f7b9aa76e9edc857a7dd62185f11b0a`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:f580883564c381d3ff4c7af87c5779bb9f7b9aa76e9edc857a7dd62185f11b0a) | `amd64` |
| `migration-20221119` | `sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1) | `amd64` |
| `migration` `migration-20221123` | `sha256:2c8e8af177cc08ae47cde2940f5cc8fbc4501d1fceab76eb5c38a06797f3804b`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:2c8e8af177cc08ae47cde2940f5cc8fbc4501d1fceab76eb5c38a06797f3804b) | `amd64` |
| `migration-20221120` | `sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb) | `amd64` |
| `migration-20221121` | `sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a) | `amd64` |
| `migration-20221122` | `sha256:ad515710302861d2c78db94aafb16fb4a280968c5517eaf14c7db88ffcddee6d`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:ad515710302861d2c78db94aafb16fb4a280968c5517eaf14c7db88ffcddee6d) | `amd64` |



## Signing

All Chainguard Images are signed using [Sigstore](https://sigstore.dev)!

<details>
<br/>
To verify the image, download <a href="https://github.com/sigstore/cosign">cosign</a> and run:

```
COSIGN_EXPERIMENTAL=1 cosign verify cgr.dev/chainguard/wolfi-base:latest | jq
```

Output:
```
Verification for cgr.dev/chainguard/wolfi-base:latest --
The following checks were performed on each of these signatures:
  - The cosign claims were validated
  - Existence of the claims in the transparency log was verified offline
  - Any certificates were verified against the Fulcio roots.
[
  {
    "critical": {
      "identity": {
        "docker-reference": "ghcr.io/chainguard-images/wolfi-base"
      },
      "image": {
        "docker-manifest-digest": "sha256:f580883564c381d3ff4c7af87c5779bb9f7b9aa76e9edc857a7dd62185f11b0a"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "f165bb9052812ac723890cb9059661d7529cab6a",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCID0bL9/Zvx4WjgOgRZTkhVAmHU/kpisXCcgbqKR3OFv+AiAIrAL8jyMW2cSDNGNb6z3BCK11P8/YCM3+YCTSs3ePiw==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJmNjY5ZDhkOGEwZDUzNmU3ZWU4ZjA0OTg4NzIwY2E0NDMxZjkyMzYzNTNiYTAxZTI2YzE1ZTczZjJhZjgxN2FlIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJQ2lIMlBSWGExUkNZZXlNZzJrY05SR2g5SDBXcENMc2U2cVRma25EbGl2V0FpRUEwUm0zQ2ZTMXNQaUJSVGpWZ2tlK3dONm9rN3ZzeVpSZzY5L0QxSllZWDRjPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUnpha05EUVhwcFowRjNTVUpCWjBsVlV6WTNWV0V4VlRCT1lWRllaamRFTm5SUGQwMXlRMUJZYzB4UmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hwTlJFRjRUbFJOTUZkb1kwNU5ha2w0VFZSSmVrMUVRWGxPVkUwd1YycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZTY2psaVNVNU9URTFtT1VWeVp5OTJWMjFVYzIxVVdXbEJRbVJFYTNaVWJTdGlhMU1LWjJOc1F6ZDVNV1IyYW10eVlYVTNSMGRoVlU5M2FHOHpSVUpoZUZsVGNUZHZUMEpGWVZabGJHNWlUVlJHVDI5VWR6WlBRMEZzWTNkblowcFVUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZWVTFSMkNtcFhaMU0zTW14Q2QwRkdkVGdyZVhacE9VcExaRGhGZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFIxbDRUbXBXYVZscWEzZE9WRWswVFZSS2FGbDZZM2xOZW1jMVRVZE9hVTlVUVRGUFZGa3lDazFYVVROT1ZFazFXVEpHYVU1dFJYZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHJSME5wYzBkQlVWRkNNVzVyUTBKQlNVVmxkMUkxUVVoalFXUlJSR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOb01YZFdia0ZCUVVWQmQwSkhUVVZSUTBsSWJsQUtlSE5xTlc1T05WQkVUSFZtWVhrMGNIQjJReXMwTTJWdmFFVklaV2swYnpOS2RtaE9WV0owVGtGcFFUbDRkMVpoUjJwNmF6TXpVM1phWTJONmFtdGFUQXBTY1dwMU9XOXdiMHhQYXpoUmRUTlhPQ3R1ZDBwNlFVdENaMmR4YUd0cVQxQlJVVVJCZDA1dlFVUkNiRUZxUlVGbk1VVjZhR3A1TlhWak1ITjNOMUZwQ2xkM1ZFbHRibEpZZEhadWJ6aFhVV1ozU1Vaa1pWa3pXVEptVFRaU1RGZDVObXBDVW1kM1JFRnhXVXhyVjNSaGVVRnFRVzlxY0RjeVNVODRORFEzVEVnS1RWVm1hMEZ2T1ZsVWRIQlVZeTlUVVhBd01WVXJhVFp4WkZNMk1IWndPVFU1T0ZSemVGZHVhRUZQYjBvMk5YaG9VRkpOUFFvdExTMHRMVVZPUkNCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2c9PSJ9fX19",
          "integratedTime": 1669162538,
          "logIndex": 7651659,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "f165bb9052812ac723890cb9059661d7529cab6a",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3528131812",
      "sha": "f165bb9052812ac723890cb9059661d7529cab6a"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

