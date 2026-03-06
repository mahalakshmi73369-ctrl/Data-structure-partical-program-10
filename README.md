# Data-structure-partical-program-10
queue = []

while True:
    print "\n1.Add Patient 2.Serve Patient 3.Display 4.Exit"
    ch = input("Enter choice: ")

    if ch == 1:
        name = raw_input("Enter patient name: ")
        queue.append(name)

    elif ch == 2:
        if len(queue) == 0:
            print "No patients"
        else:
            print "Serving:", queue.pop(0)

    elif ch == 3:
        print "Waiting list:"
        for p in queue:
            print p

    else:
        break
