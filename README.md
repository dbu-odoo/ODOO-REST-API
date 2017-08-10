REST-API
----




AVAILABLE API
----

    • Product
    • Project
    • Task
    • Employees
    • Departments
    • Job Positions
    • Employee Leaves



EMPLOYEE EXAMPLE
----

Fetch all employees using odoo REST API.



API
-------------------------

    URL     :  http://<SERVER_URL>/get/api/1.0/get/list/employees
    URL     :  http://<SERVER_URL>/get/api/1.0/get/employee/id/<EMPLOYEE_ID>
    HEADER  :  {"Authorization", "OAuth <AUTH_TOKEN>"}



REQUEST
-------------------------

    import urllib2

    request = urllib2.Request('http://<SERVER_URL>/get/api/1.0/get/list/employees')
    request.add_header("Authorization", "OAuth <AUTH_TOKEN>")
    request = urllib2.urlopen(request)
    result = request.read()



RESPONSE
-------------------------

    {u'employees': [{u'active': True,
                 u'city': False,
                 u'coach_id': False,
                 u'company_id': 1,
                 u'country_id': False,
                 u'department_id': 4,
                 u'gender': u'male',
                 u'id': 2,
                 u'job_id': 2,
                 u'marital': u'single',
                 u'name': u'Antoine Langlais',
                 u'user_id': False,
                 u'work_phone': u'+3281813700'},
                {u'active': True,
                 u'city': False,
                 u'coach_id': False,
                 u'company_id': 1,
                 u'country_id': False,
                 u'department_id': 1,
                 u'gender': False,
                 u'id': 12,
                 u'job_id': 5,
                 u'marital': False,
                 u'name': u'Ashley Presley',
                 u'user_id': False,
                 u'work_phone': u'+3281813700'}]}


*Contact me for module
