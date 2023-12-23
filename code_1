from datetime import datetime

def calculate_ages(people, year):
    def get_age(person):
        birthdate = datetime.strptime(person['birthdate'], '%Y-%m-%d')
        today = datetime(year, birthdate.month, birthdate.day)
        return today.year - birthdate.year

    return [get_age(person) for person in people]

people = [
    {'name': 'Alice', 'birthdate': '1980-01-01'},
    {'name': 'Bob', 'birthdate': '1975-02-15'},
    {'name': 'Charlie', 'birthdate': '1985-05-15'}
]

ages = calculate_ages(people, 2020)

for i, person in enumerate(people):
    print(f"{person['name']} is {ages[i]} years old in 2020.")
