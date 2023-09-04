![Abstract Booklet](pictures/ab-card.png)

## Download Functionality

By clicking the Download button, the plugin initiates a task in MEOW that produces an ODT file of the Abstract Booklet as an output.

## Settings

The abstract booklet generation settings pertain to the format of the headers and the custom fields to be included.

### Headers

![Headers](pictures/ab-headers.png)

You can customize the format for the following headers:

- Session Header 1, which is the main header
- Session Header 2, which is the subheader
- Contribution Header, which is the header for normal contributions
- Contribution Header (Poster), which is the header for contributions marked as posters

Specific placeholders must be used, such as:

- {code} for the Session/Contribution code
- {title} for the Session/Contribution title
- {start} for the Session/Contribution start date
- {end} for the Session/Contribution end date
- | (pipe) for table columns, as the contribution header is formatted as a table

### Custom Fields

![Custom Fields](pictures/ab-custom-fields.png)

By checking any of the listed custom fields, they will appear in the contribution. Custom fields are defined in the "Contributions" panel of Indico (under Organization) and can change based on the conference configuration.
