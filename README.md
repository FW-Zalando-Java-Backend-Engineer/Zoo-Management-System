## 👥 **Group Assignment: "Zoo Management System" 🦁🐘🦓**

### 🎯 **Objective:**
Build a **Java-based Zoo Management System** that models different animals, their behaviors, and basic zoo operations using the following concepts:

- ✅ Encapsulation
- ✅ Inheritance
- ✅ Polymorphism
- ✅ Method Overriding
- ✅ Git collaboration (branching, pull requests, merge conflicts)

---

### 👨‍🏫 **Storyline:**
You’ve been hired by the director of “Java Jungle Zoo” to develop a software that keeps track of the animals and simulates how they behave when visitors arrive.

---

## 🗂️ Git + Group Workflow
Each team should:
1. Create a **GitHub repo**
2. Assign tasks to 3–4 members
3. Each student works in their **own branch**
4. Push work and open a **Pull Request**
5. One member reviews and merges each PR

---

## 📋 Assignment Breakdown – 8 Tasks

### 🧑‍💻 **Member A**
#### Task 1: Create the Base Class `Animal`
- Properties (all private):
  - `name` (String)
  - `age` (int)
  - `type` (String – e.g. "Mammal", "Bird")
- Encapsulate with:
  - `getName()`, `getAge()`, `getType()`
  - `setAge()` with validation (must be > 0)
- Method: `makeSound()` – just `System.out.println("Some generic animal sound")`

#### Task 2: Create Class `Zoo`
- Maintain a `List<Animal>` called `animalList`
- Add method `addAnimal(Animal animal)`
- Add method `showAllAnimals()` to print name + type of each animal

---

### 🧑‍💻 **Member B**
#### Task 3: Create Class `Lion` that **extends Animal**
- Constructor: set `type` to `"Mammal"`
- Override `makeSound()` → `"Roar! I'm a Lion!"`

#### Task 4: Create Class `Parrot` that **extends Animal**
- Constructor: set `type` to `"Bird"`
- Override `makeSound()` → `"Squawk! I'm a Parrot!"`

---

### 🧑‍💻 **Member C**
#### Task 5: In `Zoo`, add method `simulateAnimalSounds()`
- Loop through animals, call `makeSound()` → Demonstrates **Polymorphism**

#### Task 6: Create a `Main.java` file
- Instantiate Zoo
- Add at least:
  - 1 Lion
  - 1 Parrot
- Call `showAllAnimals()` and `simulateAnimalSounds()`

---

### 🧑‍💻 **Member D**
#### Task 7: Add `feedAllAnimals()` method in Zoo
- Print `"Feeding <animal name> some food..."` for each animal

#### Task 8: Create a new animal: `Elephant`
- Extend `Animal`
- Set type `"Mammal"`
- Override `makeSound()` → `"Trumpet! I'm an Elephant!"`
- Add it to the zoo in `Main.java`

---

## 📚 Example Output:
```text
Zoo Animals:
- Leo (Mammal)
- Polly (Bird)
- Ellie (Mammal)

Animal Sounds:
Roar! I'm a Lion!
Squawk! I'm a Parrot!
Trumpet! I'm an Elephant!

Feeding Leo some food...
Feeding Polly some food...
Feeding Ellie some food...
```

---

## 🧰 Suggested Git Commands
```bash
# Everyone
git clone <repo_url>
git checkout -b feature/task-1

# After writing code
git add .
git commit -m "Completed Task 1: Created Animal class"
git push origin feature/task-1

# Open a Pull Request via GitHub
```

---

## ✅ Submission Checklist
- [ ] All tasks completed
- [ ] Each task in a separate branch
- [ ] Pull Requests created and merged
- [ ] Final version compiles and runs
- [ ] BONUS: No merge conflicts 😎

---

## 🏁 Extra Challenge (Optional)
Add a `removeAnimalByName(String name)` method to `Zoo`.

