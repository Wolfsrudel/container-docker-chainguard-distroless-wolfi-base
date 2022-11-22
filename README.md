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
| `latest` | `sha256:5491f69ec39c29ce7d32cb8af658fedfabf3355a8eb467ad64abc5fca5d869b4`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:5491f69ec39c29ce7d32cb8af658fedfabf3355a8eb467ad64abc5fca5d869b4) | `amd64` |
| `migration-20221119` | `sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:79960a947c92e8dd65628f01f407bc9b56bdf37fd4d5e5d490ed26fd1857dcb1) | `amd64` |
| `migration` `migration-20221122` | `sha256:256c2bb685feb444c20cb377c8c240aed454f3ddbd04791c5abb49f0fdcd7617`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:256c2bb685feb444c20cb377c8c240aed454f3ddbd04791c5abb49f0fdcd7617) | `amd64` |
| `migration-20221120` | `sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:6f927836f03ddf962d38d6ad7d8944e2f12051810f2e408f4c9abdb04a912afb) | `amd64` |
| `migration-20221121` | `sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:fea3bbcff3ddaa548713b209a004c7b40fe1c0a3af242a4970e8e4ad3765380a) | `amd64` |



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
        "docker-manifest-digest": "sha256:5491f69ec39c29ce7d32cb8af658fedfabf3355a8eb467ad64abc5fca5d869b4"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "3366e6329236689b2fd8a669bdc94ba25f51c801",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/wolfi-base",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQCBPuSmuPW80trO8HYP1O/Zmxil/WjlKPvg7UpZCcOh7AIgAOJvH9f4P8VzmrjGG1RD3Vt+PeTnxvlaJexq8tHEjuk=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI0YzFmNDcwZWI5ODI1NTE4N2RlNDZjMTZiMjI5OGM0NjgyZWIxOGQyZDY1NzJhNGRiYmU5YzNkYmM4NGUyZjhmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FWUNJUUN6V1Bxckp5TGtNeGNrdkRnell0eHlxd21RV3ViSnVwZGtJL1ExZjBPV1lBSWhBS2J5REtYWmo1SHNoY29mN2FBem1ORVZRRDlveU0wTEQrOWhiTUJxb2RvdSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhwdFowRjNTVUpCWjBsVlZrcHJaRkZwZGt4RVpHeHFWMkkxTURWMFlVMXhVVGxGVkRsemQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hsTlJFRjRUbXBSZWxkb1kwNU5ha2w0VFZSSmVVMUVRWGxPYWxGNlYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZhUmxOQmQxVm1hbHBNYW5sbGVsY3ljelYzWnpSMWNXdFFVeTlOWlVwRVJHTmpibmNLUkRkT2NsWkdiWGRzWkV4MFFXVjBaa1Y2UmxCdk5HeFdaMkYxYjNGdWIyMXdkVU5UZGxSaWRYUjZVbkpXY0ZFMFN6WlBRMEZzWjNkblowcFZUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZIVGs5NUNrVlhUVkJMTm5OWVRrVmxOemhZUzFaM0wyRklSVTkzZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKQldVUldVakJTUVZGSUwwSkhTWGRaU1ZwbFlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d6WkhaaVIxcHdURmRLYUdNeVZYWk1iV1J3WkVkb01WbHBPVE5pTTBweVdtMTRkbVF6VFhaamJWWnpXbGRHZWxwVE5UVlpWekZ6Q2xGSVNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcEJOVUpuYjNKQ1owVkZRVmxQTDAxQlJVSkNRM1J2WkVoU2QyTjZiM1pNTTFKMllUSldkVXh0Um1vS1pFZHNkbUp1VFhWYU1td3dZVWhXYVdSWVRteGpiVTUyWW01U2JHSnVVWFZaTWpsMFRVSlpSME5wYzBkQlVWRkNaemM0ZDBGUlNVVkRTRTVxWVVkV2F3cGtWM2hzVFVSWlIwTnBjMGRCVVZGQ1p6YzRkMEZSVFVWTFJFMTZUbXBhYkU1cVRYbFBWRWw2VG1wWk5FOVhTWGxhYlZFMFdWUlpNazlYU210WmVtc3dDbGx0UlhsT1Yxa3hUVmROTkUxRVJYZElRVmxMUzNkWlFrSkJSMFIyZWtGQ1FrRlJUMUV6U214WldGSnNTVVpLYkdKSFZtaGpNbFYzUzJkWlMwdDNXVUlLUWtGSFJIWjZRVUpDVVZGaldUSm9hR0ZYTlc1a1YwWjVXa014Y0dKWFJtNWFXRTEyWkRJNWMxcHRhM1JaYlVaNldsUkJaRUpuYjNKQ1owVkZRVmxQTHdwTlFVVkhRa0U1ZVZwWFducE1NbWhzV1ZkU2Vrd3lNV2hoVnpSM1oxbHZSME5wYzBkQlVWRkNNVzVyUTBKQlNVVm1RVkkyUVVoblFXUm5SR1JRVkVKeENuaHpZMUpOYlUxYVNHaDVXbHA2WTBOdmEzQmxkVTQwT0hKbUswaHBia3RCVEhsdWRXcG5RVUZCV1ZOamMySm1UVUZCUVVWQmQwSklUVVZWUTBsUlJIWUtUVm81TURkdU9EVkJWV0lyVTBONldFMXhSblpQTTBsNVdYaERiWFkwZGpoQ1dXVXZUVFV6U1ZaM1NXZEZTMFJVUmxGM1dWSkpWRkZNYjA5UllUZFdkd280YW1ZeE1HaENiREl6WjJkcldsWjZjbEUyTTJNMVNYZERaMWxKUzI5YVNYcHFNRVZCZDAxRVlWRkJkMXBuU1hoQlNuQmtObWh0WldaR2VtUkRMemhKQ205S04xTk9VM2hxTVhkSVNrMVBiWEpWTmpsT2VVaHhZblp5ZDNSdFFqaHFUMDFIUWtvMlFXVk5MMUJVYW5wV2RWZG5TWGhCU1d0NGFIYzBhRFoyYlhNS2VTc3dVakpDTkhaa2VUQk9iamgzUVRWMFFYTnhTRFJ5VWtwbk5GSnFabTlaWkN0WlR6ZFFja0VyY2pGQ1lVMVpOVmQxZDNwUlBUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669076207,
          "logIndex": 7576275,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/wolfi-base/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/wolfi-base",
      "githubWorkflowSha": "3366e6329236689b2fd8a669bdc94ba25f51c801",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3519202914",
      "sha": "3366e6329236689b2fd8a669bdc94ba25f51c801"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [apko](https://github.com/chainguard-dev/apko).

