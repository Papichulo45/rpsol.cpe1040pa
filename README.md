# rpsol.cpe1040pa

# Add your Python code here. E.g.
from microbit import *



rock = image ("00000:"
              "09990:"
              "09990:"
              "09990:"
              "00000:")

paper = image("99999:"
              "90009:"
              "90009:"
              "90009:"
              "99999:")

scisors = image("90099:"
                "09099:"
                "00900:"
                "09099:"
                "90099:")

lizard = image("90000:"
               "90000:"
               "90000:"
               "90000:"
               "99999:")

spock = image("99999:"
              "90000:"
              "99999:"
              "00009:"
              "99999:")

RPSLS = [rock, paper, scisors, lizard, spock]


while True:
    if accelerometer.was_gesture("shake"):
        sleep(100)
    display.show(random.choice(human_choice))
