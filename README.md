## Task
There is a certain system that handles airflights.

A flight is the transportation of a passenger from one point to another with possible intermediate landings. This means that a flight can be represented as a set of one or more elementary movements, called segments.

A segment is an atomic transportation, which for simplicity we will characterize with only two attributes: date/time of departure and date/time of arrival.

Your task is to write a module that will filter a set of flights according to various rules. There can be a lot of filtering rules. Sets of flights can also be very large. Rules can be selected and set dynamically depending on the context of the filtering operation.
## What needs to be done?
Think over the structure of the module, create the necessary classes and interfaces. If you are familiar with JUnit, cover your code with tests. Don't consider the user interface. It is enough to output information to the console. You don't need to use any third-party libraries.

## What should be taken into account?
Attached testClasses file.java contains simplified model classes and a factory for obtaining test samples. All the code must be placed in the com.package.gridnine.testing. For a test run, create a public Main class with the main() method. This method should output the results of processing the test set of flights to the console. You need to get the test set using the Flight Builder.createFlights() method.

Exclude flights according to the following rules from the test set (a separate list of flights is needed for each rule):

1. Departure before the current time.
2. Segments with arrival date before departure date.
3. Flights where the total time spent on the ground exceeds two hours (time on earth is the interval between the arrival of one segment and the departure of the next one).

## How to run the application
- Run the main method in the Main.class.
