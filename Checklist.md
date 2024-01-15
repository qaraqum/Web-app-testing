# A complete checklist for testing a web application

## Types of testing
- Usability
- Functional
- Compatibility
- Database
- Security
- Performance

## Usability testing
Verifies that the product is easy and effective to use according to standard usability testing practices.

### Usability testing scenarios
- Web page content is correct, with no grammatical or spelling errors.
- All fonts are compliant.
- All text is correctly aligned.
- All error messages are correct, with no spelling or grammatical errors, and match the window title.
- Tooltips exist for all fields.
- All fields are correctly aligned.
- Adequate space is left between fields, columns, rows, and error messages.
- All buttons should have a standard format and size.
- A link to the homepage should be on every page of the site.
- Inactive fields should be grayed out.
- Check that there are no broken links or images on the site.
- Confirmation messages should be displayed for all update and delete operations.
- Check the site at different screen resolutions ((640 x 480, 600x800, etc).
- Check that the user can use the system without annoyance.
- Check that the TAB is working properly.
- The scroll bar should only appear when it is required.
- If there is an error message when submitting a form, it should contain the information provided by the user.
- The header should appear on every page.
- All fields (text, drop-down menus, radio buttons, etc.) and buttons should be keyboard accessible and the user should be able to use the site using only the keyboard.
- Ensure that data in drop-down lists is not cut off due to field sizes, and check if the data is code-locked or admin-controlled.

## Functional testing
To ensure that the product conforms to the right functional specification mentioned in the development documentation.

### Functional testing scenarios
- Test the validation of all mandatory fields
- Ensure that the asterisk sign is displayed with all mandatory fields
- Verify that the system does not display an error window when optional fields are blank.
- Ensure that leap codes are validated correctly and do not cause calculation errors.
- Test numeric fields: they should not accept letters, in which case the corresponding error message should be displayed.
- Test negative values in numeric fields if they are allowed.
- Test that division by zero is correctly calculated.
- Test the maximum length of each field to ensure that data is not cut off.
- Test the pop-up message ("This field is limited to N characters") that should be displayed if the data entered exceeds the allowed field size.
- Verify that a confirmation message is displayed for update and delete operations.
- Verify that cost values are displayed in the correct currency.
- Test all input fields for special characters.
- Test the timeout functionality.
- Test the sorting functionality.
- Test the functionality of available buttons.
- Test the terms of use and FAQs: they should be clear and accessible to the user.
- Test that when functionality fails, the user is redirected to a dedicated error page.
- Test that all uploaded documents open correctly.
- Test that the user can download uploaded files.
- Test the mail functionality of the system.
- Test that Java Script works correctly in different browsers (IE, Firefox, Chrome, Safari, Opera).
- See what happens if the user deletes cookies while on the site.
- See what happens if the user deletes cookies after visiting the site.
- Test all the data in the drop-down lists: they should be in chronological order.
