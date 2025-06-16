# How we found states sharing personal health data with LinkedIn, Snapchat, and Google

This repo contains data for our story ["We caught 4 more states sharing personal health data with Big Tech"](https://themarkup.org/pixel-hunt/2025/06/17/we-caught-4-more-states-sharing-personal-health-data-with-big-tech).

## Methodology

The Markup and CalMatters used The Markup's [Blacklight](https://themarkup.org/blacklight) tool to scan the healthcare exchange websites of 19 states and the District of Columbia. We were looking for sites that shared personally identifying information through ad trackers and third-party cookies. Prioritizing the exchanges that had a greater than average number of trackers and cookies, we navigated each site as we watched activity in [the browser's network panel](https://developer.chrome.com/docs/devtools/network). As we filled forms on the sites, we watched for communication with the platforms that our scans had identified as ad tracker providers. Through this process, we found that the exchange sites of the five states below were sending personal health data to advertising and analytics services.

For each state, we're providing a copy of our initial Blacklight scan, screenshots of the relevant network activity in the browser's network panel, and [a HAR file](https://en.wikipedia.org/wiki/HAR_(file_format)), which documents network activity. HAR files can be read [in many modern browsers](https://help.tanium.com/bundle/HARfile-Create-Read/page/KA/HARfile-Create-Read/HARfile-Create-Read.htm) and with the [HAR Analyzer tool](https://toolbox.googleapps.com/apps/har_analyzer/).

The network traffic captured in these HAR files was generated as a Markup reporter investigated the site, entering made-up data about people that don't exist. Personally identifying information has been redacted from the HAR files. Any unredacted information that appears to be personally identifying (e.g. names, birth dates, marital status, ethnicity, race, gender) is not real.

All [the initial Blacklight scans can be found here](data/blacklight-scans/), including those for states that we didn't find sharing personal health data.

## California

Our findings for Covered California, the exchange for the State of California, are detailed in our story ["How California sent residents’ personal health data to LinkedIn"](https://themarkup.org/pixel-hunt/2025/04/28/how-california-sent-residents-personal-health-data-to-linkedin).

## Nevada

### Blacklight scan results

The [Blacklight scan results for nevadahealthlink.com](data/blacklight-scans/nevada-nevadahealthlink.com/report.md) on April 28, 2025.

### HAR file

The [HAR file for nevadahealthlink.com](data/nevada/HARs/20250519-102200-enroll.nevadahealthlink.com.har) captured on May 19, 2025.

Note: We do not have a HAR file showing the Nevada exchange site sending data to LinkedIn, as shown in the screenshots below.

### Screenshots

Showing the following information being sent to LinkedIn:

* [The name (Lipitor) and dosage (10 Mg Tab) of medication used by a member of the applying household](data/nevada/screenshots/01-nv-linkedin-medication-lipitor.png)
* [The name (Atovrastatin) and dosage (10 Mg Tab) of medication used by a member of the applying household](data/nevada/screenshots/02-nv-linkedin-medication-atorvastatin.png)
* [The name (Fluoxetine) and dosage (20 Mg Tab) of medication used by a member of the applying household](data/nevada/screenshots/03-nv-linkedin-medication-fluoxetine.png)
* [The name (Norethindrone) and dosage (0.35 Mg Tab) of medication used by a member of the applying household](data/nevada/screenshots/04-nv-linkedin-medication-norethindrone.png)
* [The name (Spironolactone) and dosage (50 Mg Tab) of medication used by a member of the applying household](data/nevada/screenshots/05-nv-linkedin-medication-spironolactone.png)

Showing the following information being sent to Snapchat:

* [The name (Fluoxetine) of medication used by a member of the applying household](data/nevada/screenshots/06-nv-snap-medication-fluoxetine.png)
* [The name (Norethindrone) of medication used by a member of the applying household](data/nevada/screenshots/07-nv-snap-medication-norethindrone.png)
* [The name (Spironolactone) of medication used by a member of the applying household](data/nevada/screenshots/08-nv-snap-medication-spironolactone.png)

## Maine

### Blacklight scan results

The [Blacklight scan results for coverme.gov](data/blacklight-scans/maine-coverme.gov/report.md) on April 28, 2025.

### HAR file

The [HAR file for coverme.gov](data/maine/HARs/20250529-152800-me25.checkbookhealth.org.har) captured on May 29, 2025.

### Screenshots

Showing the following information being sent to Google:

* [The name (Fluoxetine) and dosage (20 Mg Tab) of medication used by a member of the applying household](data/maine/screenshots/01-me-ga-medication-fluoxetine.png)
* [The name (Spironolactone) and dosage (50 Mg Tab) of medication used by a member of the applying household](data/maine/screenshots/02-me-ga-medication-spironolactone.png)
* [The name (Franklin Memorial) of a hospital used by a member of the applying household](data/maine/screenshots/03-me-ga-hospital-Franklin-Memorial.png)

## Rhode Island

### Blacklight scan results

The [Blacklight scan results for healthsourceri.com](data/blacklight-scans/rhode-island-healthsourceri.com/report.md) on April 28, 2025.

### HAR file

The [HAR file for healthsourceri.com](data/rhode-island/HARs/20250521-113600-ri25.checkbookhealth.org.har) captured on May 21, 2025.

### Screenshots

Showing the following information being sent to Google:

* [The name (Nguyen) of a doctor used by a member of the applying household](data/rhode-island/screenshots/01-ri-ga-doctor-nguyen.png)
* [The name (Smith) of a doctor used by a member of the applying household](data/rhode-island/screenshots/02-ri-ga-doctor-smith.png)
* [The name (Prozac) and dosage (20 Mg Tab) of medication used by a member of the applying household](data/rhode-island/screenshots/03-ri-ga-medication-prozac.png)
* [The name (Spironolactone) and dosage (50 Mg Tab) of medication used by a member of the applying household](data/rhode-island/screenshots/04-ri-ga-medication-spironolactone.png)

## Massachusetts

### Blacklight scan results

The [Blacklight scan results for mahealthconnector.org](data/blacklight-scans/massachusetts-mahealthconnector.org/report.md) on April 28, 2025.

### HAR file

The [HAR file for mahealthconnector.org](data/massachusetts/HARs/20250508-151600-betterhealthconnector.com.har) captured on May 8, 2025.

### Screenshots

Showing the following information being sent to LinkedIn:

* [The status (pregnant) of a member of the applying household](data/massachusetts/screenshots/01-ma-linkedin-pregnant.png)
* [The status (disabled or blind) of a member of the applying household](data/massachusetts/screenshots/02-ma-linkedin-disabled-blind.png)
