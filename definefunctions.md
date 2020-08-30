# python learning
# Functions - Returning Values Using Functions
# Return statements examples

>>> def area_triangle(base, height):
...     return base*height/2
...
>>> area_a = area_triangle(5,4)
>>> area_b = area_triangle(7,3)
>>> sum = area_a + area_b
>>> print("The sum of both areas is: " + str(sum))
The sum of both areas is: 20.5

#####

# Function "floor division symbol" means divide and take the integar // Divides a number and takes the single digit integar here is an example of this with return statement

>>> def convert_seconds(seconds):
...     hours = seconds // 3600
...     minutes = (seconds - hours * 3600) // 60
...     remaining_seconds = seconds - hours * 3600 - minutes * 60
...     return hours, minutes, remaining_seconds
...
>>>
>>> hours, minutes, seconds = convert_seconds(5000)
>>> print(hours, minutes, seconds)
1 23 20

# We may want a function to manipulate data we passed it and then return the result to us. This is where the concept of return values comes in handy. We use the return keyword in a function, which tells the function to pass data back. When we call the function, we can store the returned value in a variable. Return values allow our functions to be more flexible and powerful, so they can be reused and called multiple times.

# Functions can even return multiple values. Just don't forget to store all returned values in variables! You could also have a function return nothing, in which case the function simply exits.

>>> def circle_area(radius):
...     pi = 3.14
...     area = pi * (radius ** 2)
...     print(area)
...
>>> circle_area(5)
78.5

##### EXAMPLE:
# This function converts miles to kilometers (km).
# Complete the function to return the result of the conversion
# Call the function to convert the trip distance from miles to kilometers
# Fill in the blank to print the result of the conversion
# Calculate the round-trip in kilometers by doubling the result, and fill in the blank to print the result


# 1) Complete the function to return the result of the conversion
>>> def convert_distance(miles):
...     km = miles * 1.6  
# approximately 1.6 km in 1 mile
>>> my_trip_miles = 55
# 2) Convert my_trip_miles to kilometers by calling the function above
>>> my_trip_km = 55 * 1.6
# 3) Fill in the blank to print the result of the conversion
>>> print("The distance in kilometers is " + str(my_trip_km))
The distance in kilometers is 88.0

# 4) Calculate the round-trip in kilometers by doubling the result,
#    and fill in the blank to print the result
>>> print("The round-trip in kilometers is " + str(my_trip_km * 2))
The round-trip in kilometers is 176.0

##### Example 

# This function compares two numbers and returns them
# in increasing order.
>>> def order_numbers(number1, number2):
	if number2 > number1:
		return number1, number2
	else:
		return number2, number1

# 1) Fill in the blanks so the print statement displays the result
#    of the function call
>>> smaller, bigger = order_numbers(100, 99)
>>> print(smaller, bigger)






