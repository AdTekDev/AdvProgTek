
# W06 - Routine [2]

Implement the process of booking a hotel room using the **getRooms** method from the **HotelLocation** class, along with checking the availability of a room at a given time using the **isRoomAvailable** method from the **Room** class

## HotelLocation Class
Method 1: **getRooms**

### **Parameters**

- roomType (Type: String) - The type of room the guest is looking for (e.g., "Single", "Double", "Suite").  
- checkinDate (Type: Date) - The check-in date specified by the guest.
- checkoutDate (Type: Date) - The check-out date specified by the guest.

### **Description**
This method should take in the room type and dates as parameters and return a list of available rooms that match the requested room type and are available for booking between the check-in and check-out dates. It should make use of the isRoomAvailable method of the Room class to check each room's availability for the specified date range.

## Room Class
Method 2: **isRoomAvailable**

### **Parameters**

- checkinDate (Type: Date) - The check-in date to be checked for availability.
- checkoutDate (Type: Date) - The check-out date to be checked for availability.

### **Description**
This method should check whether the room is available for booking during the specified date range. It should return a boolean value (true or false) to indicate whether the room is available or not. The method should compare the check-in and check-out dates provided with the room's existing bookings to determine availability.
