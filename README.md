# data
def get_student_information():
    print("School Registration Form")
    print("------------------------")

    # Get student information
    student_info = {}
    student_info['name'] = input("Full Name: ")
    student_info['dob'] = input("Date of Birth (YYYY-MM-DD): ")
    student_info['grade'] = input("Grade: ")
    student_info['address'] = input("Address: ")
    student_info['parent_name'] = input("Parent's Name: ")
    student_info['contact_number'] = input("Contact Number: ")

    return student_info

def print_registration_confirmation(student_info):
    print("\nRegistration Confirmation")
    print("------------------------")
    print(f"Name: {student_info['name']}")
    print(f"Date of Birth: {student_info['dob']}")
    print(f"Grade: {student_info['grade']}")
    print(f"Address: {student_info['address']}")
    print(f"Parent's Name: {student_info['parent_name']}")
    print(f"Contact Number: {student_info['contact_number']}")
    print("\nThank you for registering!")

def main():
    student_info = get_student_information()
    print_registration_confirmation(student_info)

if __name__ == "__main__":
    main()
