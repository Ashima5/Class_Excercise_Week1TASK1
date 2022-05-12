def add():
    name=input("Enter name of student")
    grade=int(input("Enter grade of student"))
    class_record[name]=grade
    print("Name has been added to record")
    print(class_record)
    return class_record

def search():
    name=input("Enter name of student you want to search")
    if name in class_record.keys():
        print("Grade of",name,":",class_record[name])
    else:
        print("Name not in record")
    return class_record

def delete():
    name=input("Enter name of student to be deleted")
    if name in class_record.keys():
        class_record.pop(name)
        print("Name has been deleted")
    else:
        print("Name not in list")
    return class_record
            
def update():
    name=input("Enter name of student to update")
    if name in class_record.keys():
        option=int(input("enter 1 to update name or 2 to update grade"))
        if option==1:
            grade= class_record[name]
            new_name=input("Enter new name")
            class_record.pop(name)
            class_record[new_name]=grade
            print("New name updated as", class_record)
        elif option==2:
            new_grade=input("Enter new grade")
            class_record[name]=new_grade
            print("New grade updated as",class_record)
    else:
        print("Name not found")
    return class_record
                      
class_record= {}
while True:
    task=int(input("""You can perform the following operations:
Enter
    1 to add name and grade,
    2 to search name,
    3 delete name and
    4 to update name and grade
    """))
    if task==1:
        add()
    if task==2:
        search()
    if task==3:
        delete()
    if task==4:
        update()
