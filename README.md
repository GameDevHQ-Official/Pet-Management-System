# Pet Management System

## Objective

Create a text-based pet management system in C++ where players can feed, play, and care for their pets, affecting their pets' stats like happiness, health, and hunger.

## Requirements

### Pet Attributes

- Use a `struct` or `class` to define pet attributes such as name, happiness, health, and hunger.
- Implement member functions to display and update pet stats.

### Actions

- Implement functions for actions such as feeding, playing, and caring for the pet. Each action should affect the pet's stats.

### Inventory Management

- Use `std::vector` to manage the player's inventory of pet care items.
- Implement a function to use items from the inventory to affect the pet's stats.

### Items

- Define various items that can be used to care for the pet, such as food, toys, and medicine.
- Each item should have a name, an effect, and a value.

### Item Table

| Item Name    | Effect     | Value |
|--------------|------------|-------|
| Health Potion| Health     | +20   |
| Toy Ball     | Happiness  | +15   |
| Food         | Hunger     | -20   |
| Medicine     | Health     | +30   |
| Treat        | Happiness  | +10   |

### UML Design

#### Pet Class UML

```plaintext
+---------------------------------+
|             Pet                 |
+---------------------------------+
| - name: std::string             |
| - happiness: int                |
| - health: int                   |
| - hunger: int                   |
+---------------------------------+
| + Pet(name: std::string)        |
| + displayStats(): void          |
| + feed(amount: int): void       |
| + play(duration: int): void     |
| + care(time: int): void         |
+---------------------------------+
```
#### Item Class UML

```plantext
+---------------------------------+
|             Item                |
+---------------------------------+
| - name: std::string             |
| - effect: std::string           |
| - value: int                    |
+---------------------------------+
| + Item(name: std::string,       |
|   effect: std::string, value: int) |
| + use(pet: Pet&): void          |
+---------------------------------+
```
## Steps

### 1. Set Up Project
- Create a new C++ project and set up your development environment.
- Include necessary headers (`<iostream>`, `<vector>`, `<string>`).

### 2. Define Pet Class
- Create a `Pet` class with attributes: `name`, `happiness`, `health`, and `hunger`.
- Implement member functions to display and update pet stats.

### 3. Define Item Class
- Create an `Item` class with attributes: `name`, `effect`, and `value`.
- Implement a function to use items from the inventory to affect the pet's stats.

### 4. Implement Pet Actions
- Implement functions for actions such as feeding, playing, and caring for the pet.

### 5. Implement Inventory System
- Use `std::vector` to manage the player's inventory of pet care items.
- Implement functions to add items to the inventory and use them on the pet.


## Example User Interaction

```plaintext
*****************************************************************
*                    Virtual Pet Management                     *
*****************************************************************

Enter your pet's name: Fluffy
Fluffy's Stats:
- Happiness: 50
- Health: 50
- Hunger: 50

Enter 'p' to play, 'c' to care, 'i' to use item, 'q' to quit: p
Enter play duration: 30
Playing with Fluffy... Fluffy's happiness increased by 30!

Fluffy's Stats:
- Happiness: 80
- Health: 50
- Hunger: 50

Enter 'p' to play, 'c' to care, 'i' to use item, 'q' to quit: c
Enter care time: 15
Caring for Fluffy... Fluffy's health increased by 15!

Fluffy's Stats:
- Happiness: 80
- Health: 65
- Hunger: 50

Enter 'p' to play, 'c' to care, 'i' to use item, 'q' to quit: i
Inventory:
1. Health Potion (Health +20)
2. Toy Ball (Happiness +15)
3. Food (Hunger -20)
4. Medicine (Health +30)
5. Treat (Happiness +10)

Enter the item number to use: 1
Using Health Potion on Fluffy... Fluffy's health increased by 20!

Fluffy's Stats:
- Happiness: 80
- Health: 85
- Hunger: 50

Enter 'p' to play, 'c' to care, 'i' to use item, 'q' to quit: q
*****************************************************************
*                      Thanks for playing!                      *
*****************************************************************
```
## Submission Details

### 1. Complete the project and ensure it is bug-free.

### 2. Add the completed project to your GitHub repository.

### 3. Submit the link to your repository through your program dashboard to continue the program.

### 4. A code review will be processed once the submission is received.

