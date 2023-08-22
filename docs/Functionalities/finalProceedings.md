![Final Proceedings](pictures/fp-card.png)

## Site functionality

By clicking on the "Site" button, a Modal with more functionalities is opened.

![Final Proceedings Panel](pictures/fp-panel.png)

### Pre-Press and Final Proceedings

Both "Pre-Press" and "Final Proceedings" buttons are about the generation of the conference's proceedings, which some slight differences.

In fact, Pre-Press is: 

- including contributions that haven't been fully accepted

- not including contributions' slides if any

- performing a non-strict PDF checking

- skipping the generation of DOIs payloads

- the pointer to the contributions's DOI pages is internal

- having relative links to PDF files

The goal of Pre-Press is mainly to perform a quicker run, whereas Final Proceedings is in fact for the generation of the proceedings to be published.

Following is an example of a run.

![Final Proceedings Run](pictures/fp-run.png)

All the tasks are listed on the left, highlighting those completed, running and scheduled. 
On the right there are some some logs, containing informative messages on the current run.
On the bottom, a progress bar is showing the progress status.

If the run is successful, the panel is going to show like the following picture.

![Final Proceedings Success](pictures/fp-run-success.png)

If any blocking error occurs during the run, a message is displayed to the user, like the following example.

![Final Proceedings Error](pictures/fp-run-error.png)

### Compress

The "Compress" button is enabled only if any proceedings generation run has been completed successfully. This task compresses the generated proceeding folder, to make them available for the download.

### Download

The "Download" button is enabled only once the compressed proceedings are available. The functionality just starts the download on the web browser.

### Open

The "Open" button is enabled only if any proceedings generation run has been completed successfully. By clicking on it, it is opening a preview of the proceedings website.

## DOI functionality

The "DOI" button is enabled only if previously the DOI payload files have been generated. At the start, a task that is fetching the status of the contributions' DOIs is launched automatically in MEOW.

![DOI open](pictures/doi-open.png)

As a result, every DOI's status is listed:

![DOI successfull fetch](pictures/doi-fetch.png)

Following is the list of availalble actions:

- **Refresh**: fetches the status of the DOIs again

- **Create**: updates the status of the DOIs to "draft" (this action doesn't work if DOIs have been already published or registered)

- **Delete**: deletes the DOIs from the datacite repository (this action doesn't work if DOIs have been already published or registered)

- **Publish**: updates the status of the DOIs to "findable"

- **Hide**: updates the status of the DOIs to "hidden" (this action is changing the DOIs to registered if they have been already published once)

## Settings