# BEYONDIT Runtimes

This is the home of all runtime packages for our products.

To get access to our products contacts us.

After you got invited you can use the following powershell script to download a product runtime for a certain bc version.

```
$nuGetToken = '<PAT>'
$nugetServerUrl = 'https://nuget.pkg.github.com/byndit-runtimes/index.json'
$packageName = 'BEYONDITGmbH.BeyondCues.runtime-1-0-0-0'
$bcVersion = '23.0.0.0'

Get-BcNuGetPackage -nuGetServerUrl $nugetServerUrl -nuGetToken $nuGetToken -packageName $packageName -version $bcVersion -select Exact
```