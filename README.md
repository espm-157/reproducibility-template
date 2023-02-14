# neon4cast-example

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=563603613)

This repository is a template example for generating a forecast that is automated through GitHub actions. You can test-drive using the button above or copy the template to begin developing your own persistent example. 

## Applying this repository to a new forecast

1) Click "Use This Template" to copy this example to your Github account.  Choose "create a new repository" if you want to set up a persistent copy in your own account. From the copy, click "Code" button again and open in a codespace.
1) Modify `forecast_model.R` to make your forecast model .  Many of the components you need to generate the forecast, including downloading NOAA weather forecasts, downloading target data, generating forecast files, generating metadata, validating files, and submitting forecasts. Avoid running the `neon4cast::submit()` function at the end of `forecast_model.R` until you are ready to submit a forecast to the Challenge.  It is important that you do NOT change the name of the file.  GitHub Actions (below) is looking for this file name. Be sure to change your `model_id`
2) Commit and push the changes to `forecast_model.R` to Github. 

## Manually running forecast in GitHub actions

1) Under the actions tab, click on ".github/workflows/do_prediction.yml" on the left side.
2) Click "Run workflow", then the green "Run workflow" button. 

## Automatically running forecast in GitHub actins

The forecast in this repository is designed to run daily at 20:00 UTC.  The execution of the forecast occurs on GitHub's servers, so your local computer does not need to be turned on.  In ".github/workflow/do_prediction.yml", the lines `-cron: "* 20 * *"` define the time that the forecast is run.  In this case it is run each day at 20:00:00 UTC (note all GitHub timings are on UTC).  You can update this to run on a different schedule based on timing codes found in https://crontab.guru

To start the automated forecast generation
1) Find the file `do_predictions.yml` in the `.github/workflows` on GitHub.
2) Click the edit (pencil) button to edit the file.
3) Remove the `#` before the words "schedule" and "-cron".  See below:

Change

```
on:
  workflow_dispatch:
  #schedule:
  #- cron: "0 20 * * *"
```
to
```
on:
  workflow_dispatch:
  schedule:
  - cron: "0 20 * * *"
```

A video describing how to use GitHub actions for automated forecast generation can be found here: https://youtu.be/dMrUlXi4_Bo

## Running in mybinder

You can run this repo as a "binder".  The [mybinder.org](https://mybinder.org) project will convert the repository into an interactive Rstudio sesson for you. To create a binder.  Use the link below but replace "eco4cast/neon4cast-example.git" with your repository. This is the exact R configuration that GitHub will be using to run your forecast.  The use of mybinder is primarily for testing. 

https://mybinder.org/v2/gh/eco4cast/neon4cast-example.git/HEAD?urlpath=rstudio
