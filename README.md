# todo_list-repository
todo_list=[]
def add_task():
    task=input("Enter the task: ").strip()
    if task:
        todo_list.append(task)
        print(f"task {task} added successfully")
    else:
        print("no tasks added")
def view_task():
    if not todo_list:
        print("No tasks ")
    else:
        for index, task in enumerate(todo_list, start=1):
            print(f"{index}.{task}")
while True:
    print("1. add task")
    print("2. view task")
    print("3. exit")

    choice=input("enter your choice: ")
    if choice=='1':
        add_task()
    elif choice=='2':
        view_task()
    elif choice=='3':
        print("exit and byee")
        break
    else:
        print("not valid")
