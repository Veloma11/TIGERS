# TIGERS
Compare liones and tigers
class Animal:
    def __init__(self, species, habitat, weight, diet, lifespan):
        self.species = species
        self.habitat = habitat
        self.weight = weight
        self.diet = diet
        self.lifespan = lifespan
    
    def display_info(self):
        print(f"Species: {self.species}")
        print(f"Habitat: {self.habitat}")
        print(f"Weight: {self.weight} kg")
        print(f"Diet: {self.diet}")
        print(f"Lifespan: {self.lifespan} years")
        print()

class Lion(Animal):
    def __init__(self):
        super().__init__(
            species="Lion",
            habitat="Savannah, Grasslands",
            weight=190,  # Average weight for male lions
            diet="Carnivorous",
            lifespan=12  # Average lifespan in the wild
        )

class Tiger(Animal):
    def __init__(self):
        super().__init__(
            species="Tiger",
            habitat="Forests, Grasslands",
            weight=220,  # Average weight for male tigers
            diet="Carnivorous",
            lifespan=15  # Average lifespan in the wild
        )

def compare_animals(animal1, animal2):
    print("Comparing two animals:")
    animal1.display_info()
    animal2.display_info()

lion = Lion()
tiger = Tiger()

compare_animals(lion, tiger)
