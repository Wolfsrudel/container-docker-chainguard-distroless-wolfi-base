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
| `migration` `migration-20221120` | `sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb) | `amd64` |
| `latest` | `sha256:5c2b74fa29a39a574140833cc3fa5228494dd6d3b265a0132eaf55c2b3e8dfd2`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:5c2b74fa29a39a574140833cc3fa5228494dd6d3b265a0132eaf55c2b3e8dfd2) | `amd64` |
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
        "docker-manifest-digest": "sha256:5c2b74fa29a39a574140833cc3fa5228494dd6d3b265a0132eaf55c2b3e8dfd2"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "83619826b0522871c283220080d1bcdb547797b4",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQC/oz5yH35L8cSdU5XJvkwkZMRUDbvdLBN+ZzoOP2NeegIhAKTBEGA/wvFOFmu8KF9bMLv/+ZlvCFLjCTESjMcFuGvM",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJjNGViN2M1YWFiYzMwMTllZjA5ZjFmMWQyOTdkNWVlYzhkMzViNjZkZmVmZjY3N2E4OTgwMGRmZTU2MTMxYzdlIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJRTZ3WEpkdDhGM0Rzdk13WTYwZ3QrUkxXQ25Iajl2NTJITGZob1NPSXZ1RkFpQjhKdlhBZWxhMHdoNm80Smd4V3U3anBQdWJ5czM3bUhEa2RQWDJpZnFPL3c9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUnpha05EUVhwdFowRjNTVUpCWjBsVlIwODBWMUZuZVRWS1lUaDNWREZ4WlZkbllrRlNWbGR4UzNGSmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hkTlJFVjVUbnBKZWxkb1kwNU5ha2w0VFZSSmQwMUVSWHBPZWtsNlYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVYzWTFwdk5FVmxNamdyYjBZNVNTdFVNM2Q0YUM5cmVXOWtZMmg2YlhwVVMxaDJaRWtLUW1GWmJGWkdjSEIwVWpoS2IxbG5SVVJTYlZVcmQxbEtXRUpSYjB0M01VRm9Va3h0YjFOSVRHaEtVRUpuU1RKWGNEWlBRMEZzWjNkblowcFZUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZWWTNsaUNsSkljRXBxUjJVeFlrZzNibWhSVFZCcFIxVXlkeTlOZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFJHZDZUbXBGTlU5RVNUSlpha0V4VFdwSk5FNTZSbXBOYW1kNlRXcEpkMDFFWjNkYVJFWnBDbGt5VW1sT1ZGRXpUbnByTTFscVVYZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHZSME5wYzBkQlVWRkNNVzVyUTBKQlNVVm1RVkkyUVVoblFXUm5SR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOVGNHSklSRUZCUVVWQmQwSklUVVZWUTBsSVVtOEtVMVJzYkRremJUTnBORlZHWmtGRWNYSjJkbkI2VEcweGNISkZOazVNVTNselZWUnJTM2RhYVVGcFJVRTRibVJxUTBkS2JHZHBVSE5RTHpkNmVIUmhUZ3BxVTBwamIwbGlTV1ppSzAwMldDOHdlbGhxVmxWYVVYZERaMWxKUzI5YVNYcHFNRVZCZDAxRVduZEJkMXBCU1hkVFVWSk5TRGRtWTBWdk1GZG5LemxZQ21SelMwOVBUMGxwUzNoNmEzSXdkMlp2UVU5c1NtUm5jbFU1WkZkM1dXRnFaRFpPY25KWk1FWjZTV1JIT0VSVFZFRnFRU3RwYkcwNWFVVlFOamhwYVdrS2JWcE1ja05MTm1wMFdGUmhlV0p1Y0ZaWWJIcEpiVk5GUm0xVldrTXdiMjgxZW1SWFRHMTBkME4yWVhRd2NVaFdTMGxGUFFvdExTMHRMVVZPUkNCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2c9PSJ9fX19",
          "integratedTime": 1668907647,
          "logIndex": 7449890,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "83619826b0522871c283220080d1bcdb547797b4",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3505946729",
      "sha": "83619826b0522871c283220080d1bcdb547797b4"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

