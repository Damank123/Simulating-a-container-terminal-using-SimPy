# Simulating-a-container-terminal-using-SimPy
The objective of this project is to create a simulation of a container terminal using SimPy to demonstrate the ability to translate described logic into code and assess code quality using best practices, preferably an object-oriented approach.
Task Breakdown

    Vessel Arrivals:
        Vessels arrive at the terminal following an exponential distribution with an average inter-arrival time of 5 hours.
        Each vessel carries 150 containers to be discharged.

    Berthing Process:
        The terminal has 2 berths (berth_1 & berth_2). Vessels wait if both berths are occupied.
        Vessels use 1 quay crane for unloading, with 2 quay cranes available to operate on any berth.

    Unloading and Transportation:
        Each container takes 3 minutes to be lifted by a quay crane and placed onto a terminal truck.
        The terminal has 3 trucks, which transport containers to yard blocks, taking 6 minutes for a round trip.

    Simulation Events Logging:
        Print statements log events such as vessel arrivals, berthing, container moves, etc., including the current simulation time (env.now).

    Berth Release:
        Once all containers are unloaded, the vessel leaves, freeing the berth for the next vessel.

    Simulation Execution:
        The simulation runs for a user-defined period (SIMULATION_TIME), assuming 1 tick = 1 minute.
