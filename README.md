# GitHub Rock Scoop Bucket

[![Tests](https://github.com/Sayanthrock-Developer/GitHub-Rock-scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/Sayanthrock-Developer/GitHub-Rock-scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/Sayanthrock-Developer/GitHub-Rock-scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/Sayanthrock-Developer/GitHub-Rock-scoop-bucket/actions/workflows/excavator.yml)

Scoop bucket for **GitHub Rock** and its official Windows releases.

## Install

Once a Windows portable release is published:

~~~pwsh
scoop bucket add github-rock https://github.com/Sayanthrock-Developer/GitHub-Rock-scoop-bucket
scoop install github-rock
~~~

## Update

~~~pwsh
scoop update github-rock
~~~

## Development

- Scoop manifests live in bucket/.
- Run bin/test.ps1 to execute the bucket test suite.
- Run bin/checkver.ps1 to check manifest versions.
- Run bin/checkhashes.ps1 to validate hashes.
- Run bin/checkurls.ps1 to validate download URLs.
- Run bin/formatjson.ps1 to format manifests.

A release manifest is intentionally not added until GitHub Rock has a published Windows portable artifact. This keeps the bucket free of non-functional or placeholder package definitions.
