###################
# firstassignment #
###################

This is an automated test using Cypress io.

Solution:
	The test verifying a scenario works fine with four(4) spec files:

	"1-visit_login_spec" file is based on "https://www.bayzat.com" url and verifying these steps:
		visit www.bayzat.com
		log in via login link reachable from top menu

	"2-dashboard_viewteam_spec" file is based on "https://www.bayzat.com" url and verifying these steps:
		once logged in, user will land on https://www.bayzat.com/enterprise/dashboard
		"View Team" page should display list of employees (might be empty)
		New employee can be added using toolbar button above employees list (Add single employee)

	"3-add_employee_spec" file is based on "https://www.bayzat.com/enterprise/dashboard/employees/create" url and verifying this step:
		Add single employee

	"4-delete_employee_spec" file is based on "https://www.bayzat.com/enterprise/dashboard/employees/create" url and verifying these steps:
		once employee is added, she can be selected on the view employee screen
		once selected Employee can be deleted using "Delete" button that should show up near search field
		once deleted Logout using left menu user should land on www.bayzat.com again and login link should be available

How to run test:

	Using with cypress cli.


Bugs:
	There is no bug detected except one supposition. scenario say: "View Team" page should display list of employees (might be empty). 
	But there is always one emplooye which cannot deleted because of priority   

Cypress video record found at link:

	https://dashboard.cypress.io/#/projects/npbgqt/runs

Note: user.json file is not included project due to security. You must put it into directory "\cypress\fixtures" manually.(Near employee.json)

Best Regards