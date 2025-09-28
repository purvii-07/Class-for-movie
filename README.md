# Class-for-movie
#Program to create a class Movie with attributes. Store details of at least 5 movie in a list and released after 2015.

class Movie:
    def __init__(self,title,actor,director,year):
        self.title = title
        self.actor = actor
        self.director = director
        self.year = year
    def display(self):
        print("Title:",self.title)
        print("Actor:",self.actor)
        print("Director:",self.director)
        print("Year:",self.year)

movies = [
    Movie("Movie A","Actor1","Director1",2014),
    Movie("Movie B","Actor2","Director2",2016),
    Movie("Movie C","Actor3","Director3",2017),
    Movie("Movie D","Actor4","Director4",2020),
    Movie("Movie E","Actor5","Director5",2022),
]
print("\nMovies released after 2015:")
for m in movies:
    if m.year > 2015:
        m.display()
