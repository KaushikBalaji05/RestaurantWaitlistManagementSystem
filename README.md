# Restaurant Waitlist System

This is a simple C project that simulates how a restaurant manages its waitlist and tables.

## What it does

* Adds customers (parties) to a waitlist
* Seats them based on table availability
* Manages tables using a smart approach
* Allows cancelling and prioritizing (VIP) customers
* Shows estimated waiting time

## How it works

* Waitlist is handled using a **queue (linked list)**
* Tables are stored using a **binary search tree (BST)** based on capacity
* The system tries to find the best table for each party

## Files in this project

* `main.c` → runs the program and menu
* `restaurant.c` → contains all functions
* `restaurant.h` → structure definitions and declarations

## How to run

Open terminal in the project folder and run:

```
gcc main.c restaurant.c -o restaurant
./restaurant
```

## Features

* Add a new party
* Seat next party
* View current waitlist
* Estimate wait time
* View all tables
* Free a table
* Cancel a reservation
* Mark a party as VIP

## Notes

* Each party’s waiting time is estimated as `size × 5 minutes`
* VIP customers are moved ahead in the list
* Tables are assigned based on availability and size

---

This project was made as part of a Data Structures mini project to practice linked lists and trees in a real-world scenario.
