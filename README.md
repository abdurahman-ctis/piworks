# User Interface Specification Document
![Image](https://lists.office.com/Images/969df1bb-97b6-44ef-9108-dc18a5fd96c2/298428f6-6729-4501-a9de-dcaf554877fe/T4JRHA4Y8E2E91ER9XU0TNKHPD/c2f1cb7e-5022-433a-93a2-1ac0b6ec1015)

# Requirements

* A toolbar on the top of the page which includes the following:
  * New User button
  * Checkbox to un/hide disabled users
  * Save User button
* Screen below will be split into 2 parts by a vertical separator. It will include 2 screens, namely:
  * A table with field filters that will display the users
  * A form with necessary fields and validation that will add a new User. A user type should also be written, one of Guest/Admin/Superadmin

# Details

1. Toolbar:
  * New User button should be alinged to the left, with blue background
  * Checkbox should be right next to New User button
  * Save User button should be on the right, and be disabled initially
2. Left screen (Table):
  * Field names should have strong blue background
  * Actual entries will have alternating colors for UX when picking entries
  * Filter options to be placed as icons next to their respective fields
3. Right screen (Form):
  * Include name of the field followed by input field
  * User roles field should be a dropdown

# Behavior

* When new user button is clicked, the right screen form appears. After user successfully fills all fields, Save User button is enabled and can be clicked to add the user into system and display it on the table.
* Hide Disabled Users button will filter out disabled user once clicked. Action should be UI-only to reduce server load
* Table will always be shown, with default filter of ascending ID
* Filters can then be changed and ordered differently
* When a user is clicked their details get filled to form for editing.
