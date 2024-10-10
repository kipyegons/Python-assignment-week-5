# Python-assignment-week-5
# file_handling_assignment.py

# Task 1: Create a new text file and write to it
with open("my_file.txt", "w") as file:
    file.write("Hello, this is line 1.\n")
    file.write("This is line 2.\n")
    file.write("The number is 123.\n")
# Task 2: Read the contents and display them
with open("my_file.txt", "r") as file:
    content = file.read()
    print(content)
# Task 3: Append more lines to the file
with open("my_file.txt", "a") as file:
    file.write("Appending line 4.\n")
    file.write("Here's line 5.\n")
    file.write("Lastly, line 6.\n")
# Task 4: Error handling with try, except, and finally
try:
    with open("my_file.txt", "r") as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("The file was not found.")
except PermissionError:
    print("You do not have permission to read this file.")
finally:
    print("File operation complete.")
# file_handling_assignment.py

# Task 1: Create a new text file and write to it
with open("my_file.txt", "w") as file:
    file.write("Hello, this is line 1.\n")
    file.write("This is line 2.\n")
    file.write("The number is 123.\n")

# Task 2: Read the contents and display them
try:
    with open("my_file.txt", "r") as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("The file was not found.")
except PermissionError:
    print("You do not have permission to read this file.")
finally:
    print("File operation complete.")

# Task 3: Append more lines to the file
with open("my_file.txt", "a") as file:
    file.write("Appending line 4.\n")
    file.write("Here's line 5.\n")
    file.write("Lastly, line 6.\n")

# Task 4: Error handling with try, except, and finally
try:
    with open("my_file.txt", "r") as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("The file was not found.")
except PermissionError:
    print("You do not have permission to read this file.")
finally:
    print("File operation complete.")
