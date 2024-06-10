### Workflow Documentation: Generating and Sending E-Slips

**Objective:**
To automate the process of creating and sending e-slips to all employees using Google Sheets, Google Docs, and Gmail.

### Step-by-Step Process

#### 1. Prepare the Data in Google Sheets

1. **Create a Spreadsheet:**
   - Open Google Sheets and create a new spreadsheet.
   - Create columns for employee details such as `Employee Name`, `Email`, `Salary`, and any other relevant details.

2. **Enter Employee Data:**
   - Populate the spreadsheet with the necessary employee information.

#### 2. Create the E-Slip Template in Google Docs

1. **Open Google Docs:**
   - Create a new document in Google Docs.

2. **Design the E-Slip:**
   - Format the document to include placeholders for employee details. Use `{{placeholder}}` syntax for placeholders (e.g., `{{Employee Name}}`, `{{Salary}}`).

3. **Save the Template:**
   - Save the document as your e-slip template.

#### 3. Use Google Sheets and Google Docs for Mail Merge

1. **Install the Add-ons:**
   - In Google Sheets, install the **"Autocrat"** add-on.
   - In Google Docs, you might also need **"Doc Variables"** or similar for placeholders.

2. **Configure Autocrat in Google Sheets:**
   - Open your employee data spreadsheet.
   - Go to `Add-ons` > `Autocrat` > `Launch`.
   - Click on `New Job`.

3. **Setup the Merge Job:**
   - **Job Name:** Name your job (e.g., "E-Slip Generation").
   - **Choose Template:** Select the e-slip template created in Google Docs.
   - **Map Fields:** Map the placeholders in the template to the corresponding columns in your Google Sheets.

4. **Set the Destination:**
   - Choose a folder in Google Drive where the generated e-slips will be saved.

5. **Naming Convention:**
   - Define how the generated files will be named (e.g., `{{Employee Name}}_E-Slip`).

6. **Run the Job:**
   - Click `Run Job` to generate the e-slips for all employees.

#### 4. Send E-Slips via Gmail

1. **Install the Yet Another Mail Merge (YAMM) Add-on:**
   - In Google Sheets, install **"Yet Another Mail Merge (YAMM)"**.

2. **Prepare the Email Draft:**
   - In Gmail, compose a new email draft that will be used for the e-slips email.
   - Include placeholders in the draft (e.g., `{{First Name}}`, `{{Attachment}}`).

3. **Configure YAMM:**
   - Go to Google Sheets > `Add-ons` > `Yet Another Mail Merge` > `Start Mail Merge`.
   - Choose the draft email created in Gmail.
   - Map the placeholders in your email draft to the columns in your spreadsheet.

4. **Attach E-Slips:**
   - Make sure to attach the generated e-slips from Google Drive to the corresponding email.

5. **Send the Emails:**
   - Review the email settings and send the emails.

### Summary

By following these steps, you will be able to generate personalized e-slips for all employees and send them via email efficiently. This workflow leverages Google Sheets for data management, Google Docs for creating e-slip templates, and Gmail for mass email sending, ensuring an organized and automated process.

### Additional Tips

- **Testing:** Run a test with a few entries to ensure that the workflow is functioning correctly.
- **Security:** Ensure that sensitive information is handled securely and access to the Google Sheets and Docs is restricted to authorized personnel only.
- **Updates:** Regularly update the templates and data in Google Sheets to reflect any changes in employee information or salary details.

This documentation provides a clear and structured approach to automate the generation and distribution of e-slips, making the process efficient and error-free.
