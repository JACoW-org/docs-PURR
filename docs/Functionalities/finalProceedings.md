![Final Proceedings](pictures/fp-card.png)

## Site functionality

By clicking on the "Site" button, a Modal with more functionalities is opened.

![Final Proceedings Panel](pictures/fp-panel.png)

### Pre-Press and Final Proceedings

Both the 'Pre-Press' and 'Final Proceedings' buttons are related to the generation of the conference's proceedings, with some slight differences.

In fact, 'Pre-Press' involves:

- including contributions that haven't been fully accepted
- excluding contributions' slides, if any
- performing a non-strict PDF check
- skipping the generation of DOI payloads
- pointing to the contributions' DOI pages internally
- having relative links to PDF files

The main goal of 'Pre-Press' is to perform a quicker run, while 'Final Proceedings' is intended for the generation of the proceedings to be published.

Below is an example of a run.

![Final Proceedings Run](pictures/fp-run.png)

All the tasks are listed on the left, highlighting those completed, running, and scheduled.
On the right, there are logs containing informative messages on the current run.
At the bottom, a progress bar shows the progress status.
If the run is successful, the panel will appear as shown in the following picture:


![Final Proceedings Success](pictures/fp-run-success.png)

If any blocking error occurs during the run, a message is displayed to the user, as shown in the following example:

![Final Proceedings Error](pictures/fp-run-error.png)

### Compress

The "Compress" button is enabled only if any proceedings generation run has been completed successfully. This task compresses the generated proceeding folder to make them available for download.

### Download

The "Download" button is enabled only once the compressed proceedings are available. This functionality initiates the download in the web browser.

### Open

The "Open" button is enabled only if any proceedings generation run has been completed successfully. By clicking on it, a preview of the proceedings website is opened.

## DOI Functionality

The "DOI" button is enabled only if the DOI payload files have been generated previously. At the start, a task that fetches the status of the contributions' DOIs is launched automatically in MEOW.

![DOI open](pictures/doi-open.png)

As a result, the status of every DOI is listed:

![DOI successfull fetch](pictures/doi-fetch.png)

Following is the list of available actions:

- **Refresh**: fetches the status of the DOIs again.
- **Create**: updates the status of the DOIs to "draft" (this action doesn't work if DOIs have already been published or registered).
- **Delete**: deletes the DOIs from the datacite repository (this action doesn't work if DOIs have already been published or registered).
- **Publish**: updates the status of the DOIs to "findable."
- **Hide**: updates the status of the DOIs to "hidden" (this action changes the DOIs to "registered" if they have already been published once).

## Settings

Settings for final proceedings are organized into several subsections.

### General

![Final proceedings settings: General section](pictures/settings-general.png)

This section includes general information about the conference, such as location, dates, long and short book titles, series, and series numbers. It also includes the "pre-print" label.

### Extra

![Final proceedings settings: Extra section](pictures/settings-extra.png)

This section includes the following settings:

- **Primary color**: Defines the theme of the website.

- **Host info**: Text added to the homepage, under the volumes section (as highlighted in the picture below). Markdown can be used to customize the appearance of the text.

![Final proceedings settings: Host info result](pictures/settings-host-info.png)

- **Editorial Board**: Rendered in the page footer. Markdown can be used to customize the appearance.

- **Editorial JSON**: Defines the list of editors that worked on the conference. It is a JSON array of objects: `{first_name; last_name; affiliation}`.

- **duplicate_of alias** and **CAT_publish alias**: Used to define aliases of duplicate_of and CAT_publish if needed.

### Identifiers

![Final proceedings settings: Identifiers section](pictures/settings-identifiers.png)

This section is used to define the **ISBN** and **ISSN** of the conference.

### DOI

![Final proceedings settings: DOI section](pictures/settings-DOI.png)

This section includes settings for DOI:

- **DOI API ENV**: Used to switch between *Test* and *Production*.

The following picture describes how some of these settings are used to compose the DOI URL:

![Final proceedings settings: Example of DOI URL](pictures/doi-url-example.png)

Finally, **DOI User** and **DOI Password** are the credentials to access datacite.org's APIs.

### Materials

![Final proceedings settings: Materials section](pictures/settings-materials.png)

This section manages various assets related to the proceedings, such as logos, posters, covers of the at-a-glance volume, covers of the final proceedings volume, other volumes, and custom attachments. It is organized as a grouped table. For *volumes* and *attachments*, you can sort the files to have them listed in the desired order on the proceedings website.

The materials are sourced from the conference's content in Indico. To add a material to the proceedings, simply click on the 'Add' button. This will open a new modal where you can select the desired material and section, as illustrated in the following image.

![Final proceedings settings: Add material](pictures/settings-materials-add.png)

### Table of Contents

![Final proceedings settings: Table of Contents section](pictures/settings-toc.png)

This section covers the table of contents in the proceedings volume. You can include both sessions and contributions, or choose to include only one of them. It is recommended to include only sessions for conferences with a large number of contributions. This helps to keep the table of contents concise.
