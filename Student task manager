# Student Task and Expense Manager

assignments = []
expenses = []

while True:
    print("\n===== MENU =====")
    print("1. Add Assignment")
    print("2. View Assignments")
    print("3. Mark Assignment Completed")
    print("4. Add Expense")
    print("5. View Expenses")
    print("6. Filter Expenses by Category")
    print("7. Expenses Above Amount")
    print("0. Exit")

    choice = input("Enter choice: ")

    # TO-DO LIST

    if choice == "1":
        task = input("Enter assignment: ")
        assignments.append(task)
        print("Assignment added.")

    elif choice == "2":
        print("\nAssignments:")
        for task in assignments:
            print(task)

    elif choice == "3":
        print("\nAssignments:")
        for i in range(len(assignments)):
            print(i, assignments[i])

        index = int(input("Enter assignment number completed: "))
        assignments[index] = assignments[index] + " (Completed)"
        print("Assignment marked completed.")

    # EXPENSE TRACKER

    elif choice == "4":
        item = input("Enter expense category: ")
        amount = float(input("Enter amount: "))
        expenses.append((item, amount))
        print("Expense added.")

    elif choice == "5":
        total = 0

        print("\nExpenses:")
        for item, amount in expenses:
            print(item, ":", amount)
            total += amount

        print("Total =", total)

    elif choice == "6":
        category = input("Enter category: ")

        filtered = [expense for expense in expenses
                    if expense[0].lower() == category.lower()]

        print("Matching Expenses:")
        for item, amount in filtered:
            print(item, amount)

    elif choice == "7":
        limit = float(input("Enter amount: "))

        filtered = [expense for expense in expenses
                    if expense[1] > limit]

        print("Expenses Above", limit)

        for item, amount in filtered:
            print(item, amount)

    elif choice == "0":
        print("Goodbye!")
        break

    else:
        print("Invalid choice.")