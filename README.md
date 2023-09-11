# -list-application-that-allows-users-to-add-view-update-and-delete-
tasks = []

def add_task(task):
    tasks.append(task)

def view_tasks():
    for i, task in enumerate(tasks, 1):
        print(f"{i}. {task}")

def main():
    while True:
        print("\nTo-Do List:")
        view_tasks()
        choice = input("\nOptions:\n1. Add Task\n2. Quit\nEnter choice: ")
        if choice == '1':
            task = input("Enter task: ")
            add_task(task)
        elif choice == '2':
            break

if __name__ == "__main__":
    main()
