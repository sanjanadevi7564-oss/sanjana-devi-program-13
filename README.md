students = []

def insert_end(id, name, marks):
    students.append([id, name, marks])

def insert_begin(id, name, marks):
    students.insert(0, [id, name, marks])

def insert_pos(pos, id, name, marks):
    students.insert(pos, [id, name, marks])

def delete(id):
    for s in students:
        if s[0] == id:
            students.remove(s)

def search(id):
    for s in students:
        if s[0] == id:
            print("Found:", s)

def display():
    for s in students:
        print(s)

insert_end(1,"Anu",80)
insert_end(2,"Bala",75)
insert_begin(3,"Kavi",90)
insert_pos(1,4,"Ravi",85)

print("Student List:")
display()

delete(2)
print("After Delete:")
display()

search(4)# sanjana-devi-program-13
