# Queue-p4
Practice program
queue = []
# Enqueue Operation
def enqueue():
    element = input("Enter element to insert: ")
    queue.append(element)
    print(element, "inserted into queue")
# Dequeue Operation
def dequeue():
    if len(queue) == 0:
        print("Queue is empty")
    else:
        removed = queue.pop(0)
        print(removed, "removed from queue")
# Display Operation
def display():
    if len(queue) == 0:
        print("Queue is empty")
    else:
        print("Queue elements are:", queue)
while True:
    print("\n1.Enqueue")
    print("2.Dequeue")
    print("3.Display")
    print("4.Exit")
    choice = int(input("Enter choice: "))
    if choice == 1:
        enqueue()
    elif choice == 2:
        dequeue()
    elif choice == 3:
        display()
    elif choice == 4:
        break
    else:
        print("Invalid choice")

  Output:
  Output:

1.Enqueue
2.Dequeue
3.Display
4.Exit
Enter choice: 1
Enter element to insert: 10
10 inserted into queue
Enter choice: 1
Enter element to insert: 20
20 inserted into queue
Enter choice: 3
Queue elements are: ['10', '20']
Enter choice: 2
10 removed from queue
