# A complete checklist for testing a web application

## Types of testing
1. Usability
2. Functional
3. Compatibility
4. Database
5. Security
6. Performance

## 1. Usability testing
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

## 2. Functional testing
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

## 3. Compatibility testing
To evaluate how well software works in a particular browser, under a particular OS, with other software or hardware.

### Compatibility testing scenarios
- Test the site in different browsers (IE, Firefox, Chrome, Safari, Opera) and make sure the site displays correctly.
- Make sure that the version of HTML used is compatible with the respective browser versions.
- Make sure images display correctly in different browsers.
- Make sure fonts display correctly in different browsers.
- Make sure Java Script code works in different browsers.
- Test animated GIFs in different browsers.

## 4. Database testing
- The tester must understand the functional requirements, business logic, basic application scenario, and database design.
- The tester must understand the tables, triggers, storage procedures, mapping methods, and pointers used for the application.
- The tester must understand the logic of triggers, storage procedures, display methods, and pointers.
- The tester must understand which tables are affected when insert, update and delete operations are performed in the application.

### Database testing scripts
- Check the name of the database: it should match the specification.
- Check the tables, columns, column types, and default values: these should all match the specification.
- Check if the column allows the value null.
- Check the primary and foreign key of each table.
- Test the storage procedures.
- Test whether the storage procedure is set.
- Check the name of the storage procedure.
- Check the parameter names, types, and number of parameters.
- Check if the parameters are mandatory or not.
- Test the storage procedure by removing some parameters.
- Check the database, if the output is zero - records with zero must be involved.
- Test the storage procedure by setting simple SQL queries.
- Verify that the procedure returns values.
- Test the procedure by entering test data.
- Check the behavior of each flag in the table.
- Verify that the data is properly stored in the database after each entry.
- Check the data at each update, delete, and insert operation.
- Check the length of each field. The length on the backend and frontend should match.
- Check the names of the QA, UAT, and sell databases. The names should be unique.
- Check the encrypted data in the database.
- Check the size of the database and the response time for each query.
- Check the data displayed on the frontend and make sure it matches the backend.
- Check data integrity by entering invalid values into the database.
- Check the triggers.

## 5. Security testing
Aims to find flaws and gaps in terms of application security.

### Security testing scenarios
- Ensure that pages containing important data (password, credit card number, answers to secret questions, etc.) are opened via HTTPS (SSL).
- Ensure that important information (password, credit card number) is displayed encrypted.
- Make sure password rules are enforced on all authorization pages (registration, forgot password, change password).
- Ensure that if a password is changed, the user cannot log in with the old password.
- Ensure that error messages do not contain any sensitive information.
- Make sure that if the user is logged out or the session is terminated, the user cannot use the site.
- Check access to closed and open pages of the site directly without authorization.
- Make sure the "View Source Code" option is disabled and not visible to the user.
- Make sure the user's account is locked if he/she enters the password incorrectly several times.
- Ensure that the password is not stored in a cookie.
- Ensure that if any functionality fails, the system does not display information about the application, server, or database. Instead, the appropriate error message is displayed.
- Check the site for SQL injection.
- Check user rights and roles. For example, a candidate should not be able to access the admin page.
- Make sure that important transactions are written to logs and the information can be tracked.
- Ensure that session values are displayed encrypted in the address bar.
- Ensure that cookies are stored in encrypted form.
- Test the application for resistance to bruteforce attacks.

## 6. Performance testing
To evaluate whether a system or component meets specific performance requirements.

### Performance testing scenarios
- Determining the performance, stability, and scalability of an application under different workloads.
- Determining if the current architecture can support the application under peak loads.
- Determining which configuration results in the best performance.
- Determining the bottle neck of the application and infrastructure.
- Determining if response times have changed with a new version of the application.
- Evaluating the product and/or hardware to make sure it will handle the projected load volumes.

In general, it is not possible to perform performance testing manually for a number of reasons.
To deal with it, specialized performance testing tools are used:
- [Apache JMeter](https://jmeter.apache.org/) 
- [Load Runner](https://www.microfocus.com/en-us/portfolio/performance-engineering/overview)
- [Borland Silk Performer](https://www.microfocus.com/en-us/products/silk-performer/overview)
- [WAPT](https://www.loadtestingtool.com)
- [NEO LOAD]([https://www.tricentis.com/lp/neoload-performance-load-testing-ppc)
