```
import requests
r = requests.get('https://im5.org/learning/students.php?total_students=3')

r.status_code 		# if not 200, failed
aaa = r.json()		

[
    {
        "name": "Oscar Smith",
        "age": 27,
        "gender": "Male",
        "courses": [
            {
                "course_name": "Physics",
                "course_score": 64
            },
            {
                "course_name": "Philosophy",
                "course_score": 78
            },
            {
                "course_name": "Psychology",
                "course_score": 82
            }
        ]
    },
    {
        "name": "Alice Thompson",
        "age": 22,
        "gender": "Male",
        "courses": [
            {
                "course_name": "Physics",
                "course_score": 79
            },
            {
                "course_name": "Biology",
                "course_score": 54
            },
            {
                "course_name": "Computer Science",
                "course_score": 75
            },
            {
                "course_name": "Art",
                "course_score": 66
            },
            {
                "course_name": "Music",
                "course_score": 99
            }
        ]
    }
]
```
print:
```
name: "Oscar Smith" course_name: aaa course_score: 89
...
```



```
https://im5.org/learning/pets.php?customers=2

{
    "count": 2,
    "customers": [
        {
            "name": "John",
            "mobile": "0422842379",
            "age": 71,
            "gender": "male",
            "pets": []
        },
        {
            "name": "David",
            "mobile": "0422785806",
            "age": 41,
            "gender": "female",
            "pets": [
                {
                    "age": 10,
                    "species": "dog",
                    "weight": 19.6,
                    "gender": "male"
                },
                {
                    "age": 15,
                    "species": "rabbit",
                    "weight": 26.5,
                    "gender": "male"
                },
                {
                    "age": 15,
                    "species": "hamster",
                    "weight": 7.1,
                    "gender": "male"
                }
            ]
        }
    ]
}

```
