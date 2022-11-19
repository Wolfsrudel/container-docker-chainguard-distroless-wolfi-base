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
| `latest` | `sha256:69eb94efef33270ceedbd2760972e002b98a4a4e61df884b56368ee754f920a3`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:69eb94efef33270ceedbd2760972e002b98a4a4e61df884b56368ee754f920a3) | `amd64` |
| `migration` `migration-20221119` | `sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1) | `amd64` |



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
        "docker-manifest-digest": "sha256:69eb94efef33270ceedbd2760972e002b98a4a4e61df884b56368ee754f920a3"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "afc30d60037dc16f4af20cce4178993b0b8988aa",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCIAysCQFGU/lQYAoBeb4+m6D/VMuT7Re+zAmgXnMbeWquAiA8tDy7/9RmhH7MDijrpFx7poWCGPbYW6fIUyfOD6pf3w==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI5ZDNkOGQ4NTMzZGUwZmI2M2MxYzcyOTc0NDdiOTQ0MzVmZjM4NGZjYWNkZmMxMTQyOGM3NWIxN2RiMzI4ZWYwIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJQU1semtNaGlJTnM4VHcvSUZXNHVyOXBuaDNGUk5jRW5qSklVSjUrQkpmVUFpQWovT2xUbmFJaEE2ODZHbThRY3ZSOTlCelgvWEhNSXlmQlJIaEVuNjZTOUE9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhwdFowRjNTVUpCWjBsVllsQkRTSE5DYjBVeVlrcGtORkZrVWxOSFFYZE9ORkZsVUhWUmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVUlRWTlJFVjVUa1JKTVZkb1kwNU5ha2w0VFZSRk5VMUVSWHBPUkVreFYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZQU0UwMWVub3ZNWEIwTHpSMVRGbHNhRlZyVGt4R2NVbHJRWGRyTldSNVpWaHlkazhLUTBZMFVHNVVjM0F3Uld3d1YwbFJaekpEYkZwTlYweFFlbUZyVDJFclJuZG1ZVk52U3k5dGNqRTJWM2RzUVRkR1RVdFBRMEZzWjNkblowcFZUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZ1TUZkaUNtWjFSblZxT1c1YVlsQjVNbkZuY2tKRGRtaHJaVkpGZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFIwWnRXWHBOZDFwRVdYZE5SRTB6V2tkTmVFNXRXVEJaVjFsNVRVZE9hbHBVVVhoT2VtYzFDazlVVG1sTlIwazBUMVJuTkZsWFJYZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHZSME5wYzBkQlVWRkNNVzVyUTBKQlNVVm1RVkkyUVVoblFXUm5SR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOT1prb3hUa0ZCUVVWQmQwSklUVVZWUTBsUlEzTUtLMGRCV1dSV2NDdEZhM1ZvUTBJeFVVVkhWMDV5TVVsRVdsQndORWs1VlUwM2FqRlRiRmxQY3paQlNXZGtXbk0yWTJGSE5FSjVNbmczU2xwTFN6aHlZZ3B5VTNoT2NIVjJZMFZKY214UlMyUk9WMlZrY1hoVFNYZERaMWxKUzI5YVNYcHFNRVZCZDAxRVlWRkJkMXBuU1hoQlMyaHdTREJNTmpaNVJWVlJLekF6Q2toMmVqbFBOekprU2xWRk1GUlNSWGQzY1d3ME1tMTRaVGw1T1VaTVV6Sk9WSGw2ZGtOYWNFMUpZa1phVm1oSlNVNVJTWGhCU2pKUFprRktORWxVWlVNS1lrbDFRWFJUUVUxdU9FaFhNVEpEZWpaQmFqbEtZV2R3TUdoNVJHOHlUWEE0Umt4b1YzVlpXbXQ0ZVhoMFVXNUpWVXA0YlZOM1BUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1668821070,
          "logIndex": 7384406,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "afc30d60037dc16f4af20cce4178993b0b8988aa",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3501430501",
      "sha": "afc30d60037dc16f4af20cce4178993b0b8988aa"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

