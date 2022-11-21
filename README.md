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
| `latest` | `sha256:cfbcbbaac4212fa9e05edb29bcdd8de83199bb2cb2e05ecca68b246afae28415`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:cfbcbbaac4212fa9e05edb29bcdd8de83199bb2cb2e05ecca68b246afae28415) | `amd64` |
| `migration-20221119` | `sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1) | `amd64` |
| `migration` `migration-20221121` | `sha256:657fb405d68803b190c774dc11c637b4dd2e2e458c51ce52d69fe11a03b1167b`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:657fb405d68803b190c774dc11c637b4dd2e2e458c51ce52d69fe11a03b1167b) | `amd64` |
| `migration-20221120` | `sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb) | `amd64` |



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
        "docker-manifest-digest": "sha256:cfbcbbaac4212fa9e05edb29bcdd8de83199bb2cb2e05ecca68b246afae28415"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "6e184e82628cc7a736e017f2b780984b7eb7ae48",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCHxXSmpy0M7BcRPECrlfYcxwkE7Rz72s9hJSJw9bGdC0CIQCfNdwR2uujciOkfAk55oG82JRBde5vdz3gxy+OkgE+2A==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI1MTVlMmE1NmNjZGE4ZTkyMGY4ZTM5MDk2YWRkMGNiNDIxZjdmOWZjNTNjNTc4MDcwZWE5YzFhMGM4NDNmMjdlIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJRllRRXF3Y3FacVNMekUwR2RWbWxyd1pwNk56Q3Y2NWhweDRoQitQQ204dUFpRUErNkFreGg0cmlmTzFucXJaMDVMSkI3QUlKSzNDVWRNOHVIbTFqa1hqeFAwPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUnpla05EUVhwdFowRjNTVUpCWjBsVlpWVmFlVTFYYzJRM1QzbHpTSFZ2WVRCMlVtZzFWSGxDTUVOTmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hoTlJFVjVUWHBSZVZkb1kwNU5ha2w0VFZSSmVFMUVSWHBOZWxGNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVU1YTFJM00wSTVRV3h4WW1ka09VaHNNRXhtU1c5aGFIQndaVEpLWlZkc1VWSnVSa1VLYmtoMGNVSlZXRzF3YUVGTGJYSlZVRU5IUVRWeFQzVnlSRk5LVm5jM00ycFlNRlJKU1M5dmVtMWFMMWMxVTNsbWJHRlBRMEZzWjNkblowcFZUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlY2UlVaYUNsWjZObkZ5WW01MlZVaGtkM1IwTW1WcGEyUmtTekkwZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFJGcHNUVlJuTUZwVVozbE9ha2swV1RKTk0xbFVZM3BPYlZWM1RWUmtiVTF0U1ROUFJFRTFDazlFVW1sT01sWnBUakpHYkU1RVozZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHZSME5wYzBkQlVWRkNNVzVyUTBKQlNVVm1RVkkyUVVoblFXUm5SR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOWWVVeENTa0ZCUVVWQmQwSklUVVZWUTBsQmQwVUtjRXBsZEZkUE1FeEpkbFphWTBOcVVETTBSaTlHU1VweVZURlFia3BJVW1oR2RVdHNPRU5hU0VGcFJVRTJTa2xZWjFWd1ZHRnFiV1pDU1d0dE9WSnJTd3BUT1dOcVJYUlNTbkI0YTNVdk5FaE9kMWxLSzNaUk9IZERaMWxKUzI5YVNYcHFNRVZCZDAxRVlVRkJkMXBSU1hkQ2FFOXVheTl1V1hveFRGVkdjR2RWQ2tNNFREaEZiRGx1TmpoNFJEaHFNM1ZhZUZZM2FVTlhOWEU1WWtkMlNrOUdkMnhGVWxKdFZuSmthR0lyTmtrNFlrRnFSVUZyYVROWFNqSnhaM1poTURJS01tUjFUa2hZUzJSVlRYZFZSMnBwUlRGUFRUaHNURE55YTNkcldUUllSR05VV0hCSVFXRnBkRkZ6TlhsaU9WWlJlWE5QVHdvdExTMHRMVVZPUkNCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2c9PSJ9fX19",
          "integratedTime": 1668993825,
          "logIndex": 7508682,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "6e184e82628cc7a736e017f2b780984b7eb7ae48",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3510668472",
      "sha": "6e184e82628cc7a736e017f2b780984b7eb7ae48"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

