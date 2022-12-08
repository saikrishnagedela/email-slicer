# email-slicer
list1 = []
while True:
    str1 = input("Enter email or exit to stop, print to show data: ")
    if str1 == "exit":
        break
    elif str1 == "print":
        for i in list1:
            print("username:",i[0],"and domain:",i[1].upper())
        break
    elif "@" in str1:
        l1 = list(str1.split("@"))
        list1.append(l1)
    else:
        print("Input is not valid")
