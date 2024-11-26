Assignment 4 – Part One

Fuel gauges on vehicles show how much fuel is in the tank. They do this by using fractions. For example, when you see 1/4 on the gauge, it means the tank is 25% full. When it shows 1/2, the tank is half full (50%), and when it displays 3/4, the tank is 75% full.

Now, let's create a program in a file called 'fuel.py' that asks the user to input a fraction written as X/Y. Both X and Y are whole numbers. After you enter the fraction, the program will calculate the amount of fuel in the tank as a percentage and round it to the nearest whole number. If there's 1% or less of fuel left in the tank, the program will display 'E' to show that the tank is almost empty. If there's 99% or more of fuel remaining, it will display 'F' to indicate that the tank is almost full.

Your Code must follow this structure.

def main():
    ...


def convert(fraction):
    ...


def gauge(percentage):
    ...


if __name__ == "__main__":
    main()

convert expects a str in X/Y format as input, wherein each of X and Y is an integer, and returns that fraction as a percentage rounded to the nearest int between 0 and 100, inclusive. If X and/or Y is not an integer, or if X is greater than Y, then convert should raise a ValueError. If Y is 0, then convert should raise a ZeroDivisionError.

gauge expects an int and returns a str that is:
	"E" if that int is less than or equal to 1,
	"F" if that int is greater than or equal to 99,
	and "Z%" otherwise, wherein Z is that same int.



You must comment your code! 
Assignment 4 – Part Two 

In a file called test_fuel.py, implement two or more functions that collectively test your implementations of convert and gauge thoroughly, each of whose names should begin with test_ so that you can execute your tests with:

pytest test_fuel.py


Be sure to include 
import fuel or from fuel import convert, gauge

atop test_fuel.py so that you can call convert and gauge in your tests.

Take care to return, not print, an int in convert and a str in gauge. Only main should call print.
Note that you can check with pytest whether a function has raised an exception, per docs.pytest.org/en/latest/how-to/assert.html#assertions-about-expected-exceptions.
