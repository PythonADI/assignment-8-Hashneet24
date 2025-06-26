# Assignments

### Random Student Generator
In this [directory](random_student_generator/data) is given 3 files: 
- first_names.txt
- last_names.txt
- courses.txt

Implement following classes an their methods **(don't forget constructor!)**
```python
class Course:
    """Represents course taken by student"""
    title: str
    grade: int  # 0 - 100

    def is_failed(self) -> bool:
        """This method returns falls if course grade is less than 51"""


class Student:
    """Represents student with coruses they have taken"""
    first_name: str
    last_name: str
    age: int
    courses: list[Course]

    def get_full_name(self) -> str:
        """This method returns full name of a student"""

    def calculate_gpa(self) -> float:
        """This method calculates gpa from self.courses list"""

    def get_courses_by_status(status: str) -> list[str]:
        """This method return list of courses filtered by status"""
```

- After implementing classes read all 3 files and generate random students using that data. You should randomize their **first_name**, **last_name** and **courses** with random **grades**!
- Create a list of 500 random students that have at least 10 courses passed or failed (randomize grades)
- Calculate how many students have more than 1.5, 2.5 and 3.5 GPA's
- Which student has most failed courses?
- Which student has passed the most courses?
- Which student has most failed courses but has the highest GPA?
- Which student has passed the most coureses but has lowest GPA?
- Which student has passed the most courses and has highest GPA?
- Which student has most failed coruses and has lowest GPA?

**NOTES**
- Course status can only be passed or failed, depending on grade!
- Course grade ranges from 0 to 100.
- How's GPA calculated? [See link](https://gpacalculator.net/how-to-calculate-gpa/)
