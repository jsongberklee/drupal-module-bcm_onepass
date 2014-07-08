The current version does not have default role set, 
which mean everyone will have the default "authenticate user" role once they login.
You(super administrator) would need to create role(s) and apply to user(s) as you desire.
The Bulk operation module would be helpful if you have many users to be set as a custom role.

ROLE to be created / matched => 'student', 'faculty', 'staff', by the specific Berklee OnePass 'info' or 'description' properties.

*Make sure to config line #53 of bcm_onepass.install

For future modification index
	Default user validating functions list 
	• user_login_name_validate($form, &$form_state)
	• user_login_authenticate_validate($form, &$form_state)
	• onepass_user_login_final_validate($form, &$form_state)
	• user_login_submit($form, &$form_state)
