When PURR is successfully connected to a MEOW remote instance, it is displayed as "connected" like in the following picture.

![Plugin connected](pictures/plugin-connected.png)

There will be three available buttons:

- Manage settings

- Clear MEOW folders

- Disconnect

## Manage settings

This functionality covers the settings management. Upon clicking on it, it will open a modal with an accordion of three sections:

  - [Abstract Booklet](abstractBooklet.md)

  - [PDF Check](papersCheck.md)

  - [Final proceedings](finalProceedings.md)

![Settings modal](pictures/settings-modal.png)

Each section covers the specific settings of each main functionality. To learn more about its settings, visit the functionality's dedicated page.
If the settings are incomplete, like in the first time a user connects to a MEOW instance, the settings will be "incomplete", therefore a warning message is displayed in the bottom part of the view and the functionalities are not accessible.

![Incomplete settings](pictures/settings-incomplete.png)

To save the settings, click on the "Save" button. If all the required settings are provided, the modal will be closed, otherwise an error message is displayed.

## Clear MEOW folders

This functionality deletes all the conference's folders in the MEOW instance. A confirm prompt is shown before continuing. Perform this task only if strictly necessary, as it will remove the folders for every user that is working on this conference's final proceedings.

## Disconnect

This functionality disconnects PURR from MEOW. As a result, all the user settings will also be deleted and the plugin will appear as described in [Connection to MEOW](connection.md)
