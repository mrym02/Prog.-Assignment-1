class Guest:
    '''Class representing a guest in the hotel'''
    def __init__(self, guest_id, guest_first_name, guest_last_name, guest_phone_number, guest_email, guest_date_of_birth):
        self.guest_id = guest_id
        self.guest_first_name = guest_first_name
        self.guest_last_name = guest_last_name
        self.guest_phone_number = guest_phone_number
        self.guest_email = guest_email
        self.guest_date_of_birth = guest_date_of_birth

    # Getter and setter methods
    def get_guest_id(self):
        return self.guest_id

    def set_guest_id(self, guest_id):
        self.guest_id = guest_id

    def get_guest_first_name(self):
        return self.guest_first_name

    def set_guest_first_name(self, guest_first_name):
        self.guest_first_name = guest_first_name

    def get_guest_last_name(self):
        return self.guest_last_name

    def set_guest_last_name(self, guest_last_name):
        self.guest_last_name = guest_last_name

    def get_guest_phone_number(self):
        return self.guest_phone_number

    def set_guest_phone_number(self, guest_phone_number):
        self.guest_phone_number = guest_phone_number

    def get_guest_email(self):
        return self.guest_email

    def set_guest_email(self, guest_email):
        self.guest_email = guest_email

    def get_guest_date_of_birth(self):
        return self.guest_date_of_birth

    def set_guest_date_of_birth(self, guest_date_of_birth):
        self.guest_date_of_birth = guest_date_of_birth

    # Display function
    def display_guest_info(self):
        print("Guest ID:", self.guest_id)
        print("Name:", self.guest_first_name, self.guest_last_name)
        print("Phone Number:", self.guest_phone_number)
        print("Email:", self.guest_email)
        print("Date of Birth:", self.guest_date_of_birth)

# Creating two Guest objects
guest1 = Guest(
    guest_id="G001",
    guest_first_name="Amna",
    guest_last_name="AlAli",
    guest_phone_number="050-118-4555",
    guest_email="amna.alali@hotmail.com",
    guest_date_of_birth="1990-05-15")

guest2 = Guest(
    guest_id="G002",
    guest_first_name="Ahmed",
    guest_last_name="AlAli",
    guest_phone_number="055-765-4331",
    guest_email="ahmed.alali@gmail.com",
    guest_date_of_birth="1985-10-20")

# Displaying guest information
guest1.display_guest_info()
print()  
guest2.display_guest_info()



class Receptionist:
    '''Class representing a receptionist at the hotel'''
    def __init__(self, employee_id, employee_name, employee_email, employee_salary, employee_phone_number):
        self.employee_id = employee_id
        self.employee_name = employee_name
        self.employee_email = employee_email
        self.employee_salary = employee_salary
        self.employee_phone_number = employee_phone_number

    # Getter and setter methods
    def get_employee_id(self):
        return self.employee_id

    def set_employee_id(self, employee_id):
        self.employee_id = employee_id

    def get_employee_name(self):
        return self.employee_name

    def set_employee_name(self, employee_name):
        self.employee_name = employee_name

    def get_employee_email(self):
        return self.employee_email

    def set_employee_email(self, employee_email):
        self.employee_email = employee_email

    def get_employee_salary(self):
        return self.employee_salary

    def set_employee_salary(self, employee_salary):
        self.employee_salary = employee_salary

    def get_employee_phone_number(self):
        return self.employee_phone_number

    def set_employee_phone_number(self, employee_phone_number):
        self.employee_phone_number = employee_phone_number

    # Display function
    def display_receptionist_info(self):
        print("Employee ID:", self.employee_id)
        print("Name:", self.employee_name)
        print("Email:", self.employee_email)
        print("Salary:", self.employee_salary)
        print("Phone Number:", self.employee_phone_number)

# Creating two Receptionist objects
receptionist1 = Receptionist(
    employee_id="R022",
    employee_name="Sara Ahmed",
    employee_email="sara.ahmed@gmail.com",
    employee_salary=3500.00,
    employee_phone_number="050-988-8543")

receptionist2 = Receptionist(
    employee_id="R012",
    employee_name="John Doe",
    employee_email="john.doe@gmail.com",
    employee_salary=3200.50,
    employee_phone_number="050-654-3210")

# Displaying receptionist information
receptionist1.display_receptionist_info()
print()  
receptionist2.display_receptionist_info()



class Room:
    '''Class representing a room in the hotel'''
    def __init__(self, room_number, room_type, is_smoking, room_price, room_view):
        self.room_number = room_number
        self.room_type = room_type
        self.is_smoking = is_smoking
        self.room_price = room_price
        self.room_view = room_view

    # Getter and setter methods
    def get_room_number(self):
        return self.room_number

    def set_room_number(self, room_number):
        self.room_number = room_number

    def get_room_type(self):
        return self.room_type

    def set_room_type(self, room_type):
        self.room_type = room_type

    def get_is_smoking(self):
        return self.is_smoking

    def set_is_smoking(self, is_smoking):
        self.is_smoking = is_smoking

    def get_room_price(self):
        return self.room_price

    def set_room_price(self, room_price):
        self.room_price = room_price

    def get_room_view(self):
        return self.room_view

    def set_room_view(self, room_view):
        self.room_view = room_view

    # Display function
    def display_room_info(self):
        print("Room Number:", self.room_number)
        print("Room Type:", self.room_type)
        print("Smoking Allowed:", "Yes" if self.is_smoking else "No")
        print("Room Price:", self.room_price)
        print("Room View:", self.room_view)

# Creating two Room objects
room1 = Room(
    room_number=101,
    room_type="Deluxe",
    is_smoking=False,
    room_price=500.75,
    room_view="Ocean")

room2 = Room(
    room_number=202,
    room_type="Suite",
    is_smoking=True,
    room_price=850.50,
    room_view="City")

# Displaying room information
room1.display_room_info()
print()  
room2.display_room_info()



class Cancellation:
    '''Class representing a cancellation of a hotel reservation'''
    def __init__(self, cancellation_id, cancellation_date, cancellation_reason, cancellation_is_refund, reservation_id):
        self.cancellation_id = cancellation_id
        self.cancellation_date = cancellation_date
        self.cancellation_reason = cancellation_reason
        self.cancellation_is_refund = cancellation_is_refund
        self.reservation_id = reservation_id

    # Getter and setter methods
    def get_cancellation_id(self):
        return self.cancellation_id

    def set_cancellation_id(self, cancellation_id):
        self.cancellation_id = cancellation_id

    def get_cancellation_date(self):
        return self.cancellation_date

    def set_cancellation_date(self, cancellation_date):
        self.cancellation_date = cancellation_date

    def get_cancellation_reason(self):
        return self.cancellation_reason

    def set_cancellation_reason(self, cancellation_reason):
        self.cancellation_reason = cancellation_reason

    def get_cancellation_is_refund(self):
        return self.cancellation_is_refund

    def set_cancellation_is_refund(self, cancellation_is_refund):
        self.cancellation_is_refund = cancellation_is_refund

    def get_reservation_id(self):
        return self.reservation_id

    def set_reservation_id(self, reservation_id):
        self.reservation_id = reservation_id

    # Display function
    def display_cancellation_info(self):
        print("Cancellation ID:", self.cancellation_id)
        print("Cancellation Date:", self.cancellation_date)
        print("Cancellation Reason:", self.cancellation_reason)
        print("Is Refundable:", "Yes" if self.cancellation_is_refund else "No")
        print("Reservation ID:", self.reservation_id)

# Creating two Cancellation objects
cancellation1 = Cancellation(
    cancellation_id="C001",
    cancellation_date="2024-09-01",
    cancellation_reason="Medical Emergency",
    cancellation_is_refund=True,
    reservation_id="R12289")

cancellation2 = Cancellation(
    cancellation_id="C002",
    cancellation_date="2024-09-05",
    cancellation_reason="Change of Plans",
    cancellation_is_refund=False,
    reservation_id="R12291")

# Displaying cancellation information
cancellation1.display_cancellation_info()
print()  
cancellation2.display_cancellation_info()

