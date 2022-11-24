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
| `migration-20221119` | `sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1) | `amd64` |
| `migration` `migration-20221124` | `sha256:a2b49a3a85e714d6807de63d9c40efba5c5cbdebc494b631751cbef1c49da40e`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:a2b49a3a85e714d6807de63d9c40efba5c5cbdebc494b631751cbef1c49da40e) | `amd64` |
| `migration-20221120` | `sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb) | `amd64` |
| `migration-20221121` | `sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a) | `amd64` |
| `migration-20221122` | `sha256:ad515710302861d2c78db94aafb16fb4a280968c5517eaf14c7db88ffcddee6d`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:ad515710302861d2c78db94aafb16fb4a280968c5517eaf14c7db88ffcddee6d) | `amd64` |
| `migration-20221123` | `sha256:2c8e8af177cc08ae47cde2940f5cc8fbc4501d1fceab76eb5c38a06797f3804b`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:2c8e8af177cc08ae47cde2940f5cc8fbc4501d1fceab76eb5c38a06797f3804b) | `amd64` |
| `latest` | `sha256:e3bd88c4623fe07d381894a689b97494a1df72b9c28765452e6ebb4f95c05157`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:e3bd88c4623fe07d381894a689b97494a1df72b9c28765452e6ebb4f95c05157) | `amd64` |



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
        "docker-manifest-digest": "sha256:e3bd88c4623fe07d381894a689b97494a1df72b9c28765452e6ebb4f95c05157"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "f6bb0317ab576b30c9de1cdeeff29245fa92e701",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQCgquF/APxvOif1qXIIITWz3FkMjQ4l5y6z0peW2t/M+AIgTmnNWopjkgZA+O4tiUujmRTMGAbdsPLJXGBgYuatMXw=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJmYjQxZmQxNzg3ZjVhYWM4ZmUzODYyMTk0MzExODdmZmJjODVhYmExYTdjZTI2MzI0YzBjYjMwYjJlMDMwNzNmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJQWJoVzRPdy9lc1VhV0lqYnpvRGZNb21RTHgxU1RuRVE3cWU3VDZvMWE3NEFpRUFpTjNnYzFORXRDR0ZCL3QwU3ZTR3ZGR0djTnhJM3ovcWxIUzJ6elVCSUJzPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUnpla05EUVhwdFowRjNTVUpCWjBsVlFsYzBiVEZLVFc5SWEybERkVzV5TlcwM1dESkRaM0JaYWt4VmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RCTlJFRjRUbnBGZDFkb1kwNU5ha2w0VFZSSk1FMUVRWGxPZWtWM1YycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZPY1RGRmVVOURSQ3RCS3k5Qk9FMTZUSGh1YWlzcmRpOXRiR05VVUZSQ1pFOWlWRW9LTVhnelUyeE5SVWM0VVRKRVVVVkxLMDl1YVhGTU1XTTJhVWhCZWxGUWRtWldRVmRCUm5OMmIzSnlWVGwxUVV0ME5EWlBRMEZzWjNkblowcFZUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlYxYkhBM0NqTkRObk5VVTNCeWFVc3JSRGcyYjIxRlZXVkxPVE56ZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFIxa3lXVzFKZDAxNlJUTlpWMGt4VG5wYWFVMTZRbXBQVjFKc1RWZE9hMXBYVm0xYWFrazFDazFxVVRGYWJVVTFUVzFWTTAxRVJYZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHZSME5wYzBkQlVWRkNNVzVyUTBKQlNVVm1RVkkyUVVoblFXUm5SR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOdEwzUnBiRUZCUVVWQmQwSklUVVZWUTBsUlF6TUtXRTk0Y0hCa055dGtiMUZIUmt4UGVWWkJSVVY2YVM5eVZuTlJlbVkwVFhaTlZrRm9PRGd2U21kblNXZExhVkppUTBOSlFrTnhjMlJTYzA1b1ZGaHhXZ3BwWWxSNWNVVk9lamRyVlZGalJuWllNbU52TTBnNE9IZERaMWxKUzI5YVNYcHFNRVZCZDAxRVlVRkJkMXBSU1hoQlRuVnZUemxaWmtaVEwwSkZNbEJtQ21GWEwxTk9TbkZqVFVkRU1rczBNWFZKYjJKNVN6ZFRXVlJ1UTBFd2VHaDBNbXRtU1djeWJtTkxTRlpRVjJJclNGQkJTWGRHYTJGTVptWlVNVFUwU0dvS1ExSnJUR2hFVEdkdWFHdG9OREJGYUcxUFNGb3pTVU1yU1UxUmVtMDFOMkpZYm5sd05HTnphR2RPZEVad1pqaFBlVEJ4UXdvdExTMHRMVVZPUkNCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2c9PSJ9fX19",
          "integratedTime": 1669249033,
          "logIndex": 7722392,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "f6bb0317ab576b30c9de1cdeeff29245fa92e701",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3536627771",
      "sha": "f6bb0317ab576b30c9de1cdeeff29245fa92e701"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

