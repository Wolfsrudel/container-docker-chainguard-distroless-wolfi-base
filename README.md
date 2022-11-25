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
| `migration` `migration-20221125` | `sha256:e48ee441d8c5a33c0e4ab326a7b01c21cbfd26cd32059996a4be1ca9c3b0066d`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:e48ee441d8c5a33c0e4ab326a7b01c21cbfd26cd32059996a4be1ca9c3b0066d) | `amd64` |
| `migration-20221120` | `sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb) | `amd64` |
| `migration-20221121` | `sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a) | `amd64` |
| `migration-20221122` | `sha256:ad515710302861d2c78db94aafb16fb4a280968c5517eaf14c7db88ffcddee6d`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:ad515710302861d2c78db94aafb16fb4a280968c5517eaf14c7db88ffcddee6d) | `amd64` |
| `migration-20221123` | `sha256:2c8e8af177cc08ae47cde2940f5cc8fbc4501d1fceab76eb5c38a06797f3804b`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:2c8e8af177cc08ae47cde2940f5cc8fbc4501d1fceab76eb5c38a06797f3804b) | `amd64` |
| `migration-20221124` | `sha256:a2b49a3a85e714d6807de63d9c40efba5c5cbdebc494b631751cbef1c49da40e`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:a2b49a3a85e714d6807de63d9c40efba5c5cbdebc494b631751cbef1c49da40e) | `amd64` |
| `latest` | `sha256:679ec24ab714b40cd83d2d049ecb88c99f5c5c7dd5359ed455b8e10f3e862a75`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:679ec24ab714b40cd83d2d049ecb88c99f5c5c7dd5359ed455b8e10f3e862a75) | `amd64` |
| `migration-20221119` | `sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1) | `amd64` |



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
        "docker-manifest-digest": "sha256:679ec24ab714b40cd83d2d049ecb88c99f5c5c7dd5359ed455b8e10f3e862a75"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "a313d6d98e44aa969d2cdac8ac6c6be57c0b82a0",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQCHXDoC9lLJ4YzoDGIwH0fiKD/pMdCgfYFHQ6lnBUMZqAIhAKFw063DfJQbUbshDISazdghxBN9Rm3JZEx5v8gqiwlz",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJkYTFjMTg2YWNjZDlkYjYwNDdlZDg0ZjVkZTBlZDYwMWQyMjQ0NzMyODcyMmNjZjM4MDdjY2E0N2MyODE0MDIyIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FWUNJUURvL3FMcFlIZlRHNWp4SCt6SWRob1U4NXpUL0RWdXZGY1k4eFhEVXRuTjd3SWhBTEZWanY4MDdCeVBuS01XN0VOUGlFNkZsZjYxMk9xdW5ta0lDWmpwUFI5cCIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUnpha05EUVhwdFowRjNTVUpCWjBsVlNDOTBiakp5WmpONVVuVjVWM05yT1RkTFlrRlRWSGd5UVUxcmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RGTlJFRjRUa1JKTWxkb1kwNU5ha2w0VFZSSk1VMUVRWGxPUkVreVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZ2V0RFeFZTOUxPSFZUVDFONlZYSjZkSGRZVkdkcFRIZHlka2RxWVM5MmNrZEJkWFlLVjBwcWJsaE1SRzFVY1RWbVNtNXZiWFpCT1VWTU1EVkRaRTVJZVdGUU5uWmphMm96VG01U2JYTjJZbUl6WW1RNGVHRlBRMEZzWjNkblowcFZUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZ5U0M5ckNqQlJPR0pYZFcxeGNFUjNObmxqWW5NemRUUjNZakpuZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFIwVjZUVlJPYTA1dFVUVlBSMVV3VGtkR2FFOVVXVFZhUkVwcVdrZEdhazlIUm1wT2JVMHlDbGx0VlRGT01rMTNXV3BuZVZsVVFYZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHZSME5wYzBkQlVWRkNNVzVyUTBKQlNVVm1RVkkyUVVoblFXUm5SR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOelNYSllTRUZCUVVWQmQwSklUVVZWUTBsUlEzWUtNa1JrWjNSV1JUZzBaa0ptTmpoTE1uYzVkazF0ZG1Jd2NXWXZZeTlyY1ZKamNWcEZSbWhUV25KUlNXZElMelZ2V21WUksxQkxVQ3R3Um1WM1NFdHVhQW92VmpNMlpXZGxPWEpoUzFsNk0zVnFSWHBIWXpoRE1IZERaMWxKUzI5YVNYcHFNRVZCZDAxRVduZEJkMXBCU1hkUlJYTlpVbXA0WWpSNmFVZE9jMmQyQ2taeFZIWmxaVVZoWWxFeE9FNUlkRGxQTmpOTFFsY3labVZLYVhwMlkyNVJPVXczWlhkSk9DdDZSVVJQYTB4SVpVRnFRVWx6ZGt4YU1FWmpNVEZYUzJVS1JFZ3JhVEIxUWpWV01WTk5PVWxqY21aaWFFMUVVV2h6TVZkV1NsUnJkMjlPYkdSUFVrcHpVR294VHpWM0szbGhWSE5WUFFvdExTMHRMVVZPUkNCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2c9PSJ9fX19",
          "integratedTime": 1669335269,
          "logIndex": 7791241,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "a313d6d98e44aa969d2cdac8ac6c6be57c0b82a0",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3544355360",
      "sha": "a313d6d98e44aa969d2cdac8ac6c6be57c0b82a0"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

