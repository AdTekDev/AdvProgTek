
# W07 - Routine [3]


Implement the code in C++ to check room availability based on the provided requirements:

## Room Class

### Attributes:

- **bookingList** (a list or vector) to store information about the guests who have booked the room during various time periods.

### Method: isRoomAvailable

**Parameters**:  
- **checkinDate** : The check-in date for which you want to check room availability.
- **checkoutDate** : The check-out date for which you want to check room availability.

**Return Value**:  
bool
- This method returns true if the room is available for the specified date range (between checkinDate and checkoutDate).   
- It returns false if the room is already booked during any part of the specified date range.

## RoomBooking Class

### Attributes:

- startDate - checkin (DateTime): The check-in date for the booking.
- durationDays --> (startDate + durationDays-1) checkout (DateTime): The check-out date for the booking.

### Method: checkOverlap

**Parameters**:  
- checkinDate : The check-in date to be compared for overlapping with the current booking.
- checkoutDate : The check-out date to be compared for overlapping with the current booking.

**Return Value**:  
bool
- This method returns true if there is an overlap in the booking dates between the current RoomBooking object and the specified checkinDate and checkoutDate.   
- It returns false if there is no overlap, indicating that the two date ranges do not conflict.
