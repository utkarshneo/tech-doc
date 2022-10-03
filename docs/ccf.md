# Cloud Carfon FootPrint Plugin

**Description:** View your cloud carbon footprint by estimating energy use (kilowatt-hours) and carbon emissions (metric tons CO2e) from public cloud usage in RearPortal.

-  Forecast

- Cloud Usage 

- Estimates the carbon emissions from the Services running on the Cloud.

- Carbon Intensity Map

- Recommendations 

**Business Value:**  The Idea of carbon emissions plugin is to estimate the carbon emissions from the services running on the Cloud and estimate the carbon emissions and Make Green Tomorrow for the Companies using it. 




## Plugin Deep-Dive
It analyses the carbon emissions from the services running on the Cloud and estimates the carbon emissions
and make it possible to track the Energy Consumption  of the services running on the Cloud.

### Developer Docs

Developer Docs are mentioned here: https://github.com/cloud-carbon-footprint/ccf-backstage-plugin/blob/trunk/README.md

### User Docs


The Plugin if integrated require integration with cloud Provider like Google Cloud Platform .


The CloudCarbonFootPrint Annotation will do the job automatically for catalog entities

```yaml
cloudCarbonFootprint:
  gcp:
    useBillingData: true
    billingProjectId: my-project
    billingProjectName: My Project
    bigQueryTable: billing_export_dataset.gcp_billing_export_v1_01B22A_05AA4C_87BDAC
```

### Owner of the Package

[Cloud Carbon footPrint](https://www.cloudcarbonfootprint.org/)

## Decision

**The plugin seems useful and will be part of RearPortal out-of-the-box offerings.**

The Use of the Plugin depends on the Client needs if they want to use the same for Cloud Carbon footPrint.**

