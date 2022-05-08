# gr_29_homework_Postman
#A collection with all requests for homework, exported from postman to json, can be found at the link: https://github.com/gadaborshev/gr_29_homework_Postman/blob/main/gr_29%20homework.postman_collection.json

#Задание EP_1

Protocol: http
IP: 162.55.220.72
Port: 5005
EP_1
Method: GET
EndPoint: /get_method
request url params: 
name: str
age: int

response: 
[
“Str”,
“Str”
]

#Мое решение

Отправляю запрос по get-методу:

	162.55.220.72:5005/get_method?name=Ruslan&age=41

От сервера получаю респонз:
	
	[
		"Ruslan",
		"41"
	]
==================

# Задание EP_2

Method: POST
EndPoint: /user_info_3
request form data: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}


#Мое решение

Отправляю запрос по post-методу:
	
	162.55.220.72:5005/user_info_3
	
От сервера получаю респонз:

{
    "age": "41",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "u_salary_1_5_year": 4000
    },
    "name": "Ruslan",
    "salary": 1000
}
==================

#Задание EP_3

Method: GET
EndPoint: /object_info_1
request url params: 
 name: str
 age: int
 weight: int

response: 
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}

#Мое решение 

Отправляю запрос по get-методу:

	162.55.220.72:5005/object_info_1?name=Ruslan&age=41&weight=85
	
От сервера получаю респонз:	

{
    "age": 41,
    "daily_food": 1.02,
    "daily_sleep": 212.5,
    "name": "Ruslan"
}
==================

#Задание EP_4
Method: GET
EndPoint: /object_info_2
request url params: 
 name: str
 age: int
 salary: int

response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }

#Мое решение 

Отправляю запрос по get-методу:

	162.55.220.72:5005/object_info_2?name=Ruslan&age=41&salary=1000
	
От сервера получаю респонз:	

{
    "person": {
        "u_age": 41,
        "u_name": [
            "Ruslan",
            1000,
            41
        ],
        "u_salary_5_years": 4200.0
    },
    "qa_salary_after_1.5_year": 3300.0,
    "qa_salary_after_12_months": 2700.0,
    "qa_salary_after_3.5_years": 3800.0,
    "qa_salary_after_6_months": 2000,
    "start_qa_salary": 1000
}
	
==================

#Задание EP_5
Method: GET
EndPoint: /object_info_3
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }

#Мое решение 

Отправляю запрос по get-методу:

	162.55.220.72:5005/object_info_3?name=Ruslan&age=41&salary=1000
	
От сервера получаю респонз:	
	
{
    "age": "41",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "pets": {
            "cat": {
                "age": 3,
                "name": "Sunny"
            },
            "dog": {
                "age": 4,
                "name": "Luky"
            }
        },
        "u_salary_1_5_year": 4000
    },
    "name": "Ruslan",
    "salary": 1000
}
==================

#Задание EP_6
Method: GET
EndPoint: /object_info_4
request url params: 
 name: str
 age: int
 salary: int

response: 
{'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}


#Мое решение 

Отправляю запрос по get-методу:

	162.55.220.72:5005/object_info_4?name=Ruslan&age=41&salary=1000
	
От сервера получаю респонз:	

{
    "age": 41,
    "name": "Ruslan",
    "salary": [
        1000,
        "2000",
        "3000"
    ]
}
==================

#Задание EP_7
Method: POST
EndPoint: /user_info_2
request form data: 
 name: str
 age: int
 salary: int

response: 
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }
		  
#Мое решение 

Отправляю запрос по post-методу:

	162.55.220.72:5005/user_info_2
	
От сервера получаю респонз:	

{
    "person": {
        "u_age": 41,
        "u_name": [
            "Ruslan",
            1000,
            41
        ],
        "u_salary_5_years": 4200.0
    },
    "qa_salary_after_1.5_year": 3300.0,
    "qa_salary_after_12_months": 2700.0,
    "qa_salary_after_3.5_years": 3800.0,
    "qa_salary_after_6_months": 2000,
    "start_qa_salary": 1000
}
