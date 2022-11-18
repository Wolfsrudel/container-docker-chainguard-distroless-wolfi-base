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
| `latest` | `sha256:2217d4a346503555a4f15fa61e9e28f4cc167448387d6b172d94f5c8e51f1a64`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:2217d4a346503555a4f15fa61e9e28f4cc167448387d6b172d94f5c8e51f1a64) | `amd64` |



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
        "docker-manifest-digest": "sha256:2217d4a346503555a4f15fa61e9e28f4cc167448387d6b172d94f5c8e51f1a64"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "fdfd620416382ef4e81392b3ef222414acd06c72",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCIFzuNyMmje6AevxSgM7BVY04Y3ShhTKH5WLUes8dSqDBAiAWg42NANY3gGmMhh5Dls8Xoas0W4deMaEHJLP4o5hipg==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiIyNzM1YjdlYmMyMmNmMzk3NGFlOWU0OTFjNzU3Y2QyMTllNmIzNTRiMzQ0NTM2MmJkODdiODJkMDc1YzcxZGE3In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJUURvWWdxdGl3d3dIOUp0d29ISVI1Q0xudmRjMm1WdG9Tb3g4bFFxcjBMUjBBSWdIL0JWVUtJbUlCeUhCTVBCK1lvTE9rRCtJS0NjVzhaNnY2RUNWVE9ER2N3PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUnpha05EUVhwcFowRjNTVUpCWjBsVlMxTTNOalZWWW01YWFDdElVMGhCYTBFMVZVcGlPWEFyVUdSM2QwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVUlRSTlJFVjVUMFJCTVZkb1kwNU5ha2w0VFZSRk5FMUVSWHBQUkVFeFYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVUyZW5sMmFUWTFXbU4xUnpScVNGWXdMMVp2ZG10d1YwOTBTeTlUUkcxcVZ6bGFOMmNLWWxWT1NHNUxWWEl3WjFobEswSlVNa2x5YkdacVpYUktWRXMyVjB0VllVYzBObkZ1ZVdsV05rWjVUR1pIWldKTllVdFBRMEZzWTNkblowcFVUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlVyYWxWQ0NsYzNhbFJaTXpOelkyUmtaMHBVUVRoeFpUQm1kRGcwZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFIxcHJXbTFSTWsxcVFUQk5WRmw2VDBSS2JGcHFVbXhQUkVWNlQxUkthVTB5Vm0xTmFrbDVDazVFUlRCWlYwNXJUVVJhYWs1NlNYZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHJSME5wYzBkQlVWRkNNVzVyUTBKQlNVVmxkMUkxUVVoalFXUlJSR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOSlYxbzFNa0ZCUVVWQmQwSkhUVVZSUTBsQlZ6a0tkVkEzWlcweE5rdzFkeXQ2V0dGVGRWRlFNVkZ1VlZWRVRYTk9lVlY2Y21oQ2J5OUplbWRzUkVGcFFUTjJiVlkxYkhwSGEycFlUVUlyU1RWRk0wcGFXZ3BNTTNoRE1sQkZjM3BrZUVGMVFuVjVPWEp5YVdWNlFVdENaMmR4YUd0cVQxQlJVVVJCZDA1dlFVUkNiRUZxUW5WbllqUTRTRWhKUlU0dkwzQnBjWGxSQ2tZMWNEaHVkbUZVZEc1NEwyaENRaTlOUlVzMlpEVmtWa3RxVEhOWE9VbzFjMkU0VEdGTVdFUkZhbU4yVjBsclEwMVJRM0pEVW1ReFMzTXdTbkJ4VWxrS2NrOHdZVEpFUkhoU2IwaGlUMGxFVURCNE9EWmlOMHhoUW01RlVXRlpRekJXYjI5MFoxb3JWMUpsUkdaM2VWcHpLMVZGUFFvdExTMHRMVVZPUkNCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2c9PSJ9fX19",
          "integratedTime": 1668734890,
          "logIndex": 7311548,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "fdfd620416382ef4e81392b3ef222414acd06c72",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3493409373",
      "sha": "fdfd620416382ef4e81392b3ef222414acd06c72"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

