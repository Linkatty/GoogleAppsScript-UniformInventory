# GoogleAppsScript-UniformInventory
JavaScript code for App Script that will send an email with items in the poor condition and their quantity.
# Yacht Uniform Management System (Google Apps Script)

A Google Apps Script solution for yacht uniform management. This script is designed to automatically send an email listing uniform items in 'Poor' condition.

## Features

- **Automated Email Notifications**: Automatically sends an email listing all uniform items that are in 'Poor' condition.
- **Centralized Management**: All uniform data is managed within a Google Sheet, offering a user-friendly interface for data input and modification.

## Setup

1. **Google Sheet Setup**:
    - Create a Google Sheet with the following columns:
        - Item ID
        - Uniform Type
        - Size
        - Condition
        - Date Acquired
        - Last Inspection Date
        - Quantity
        - Notes

2. **Google Apps Script Setup**:
    - Open the Google Sheet.
    - Navigate to `Extensions` > `Apps Script`.
    - Paste the provided script into the editor.
    - Save your changes.

3. **Run & Authorize the Script**:
    - In the Google Apps Script editor, select the `sendEmailForPoorConditionItems` function from the dropdown.
    - Click the play/run button (triangle icon).
    - Google will request permissions to manage your spreadsheets in Google Drive and view and manage your email. Grant the required permissions.

4. **Automate the Script** (Optional):
    - If you wish to automate the email sending process, set up a time-driven trigger via the Apps Script dashboard.

## Usage

- Simply update the Google Sheet with uniform inventory data. 
- When the `sendEmailForPoorConditionItems` function is run (either manually or via a trigger), it will automatically send an email with a list of all items in 'Poor' condition to the specified recipient.

## Customization

- **Recipient Email Address**: Change the `recipients` constant in the script to the desired recipient email address.
- **Email Subject & Body**: Adjust the `subject` and `emailBody` variables in the script as required.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)

