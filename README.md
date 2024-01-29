# Anti_Fire_FREE-
Hello! This is a Free Website because your struggling to get through school.
I know that we hate () so do you
from termcolor import colored
# we will need this package for rainbow text
import sys, time, random
# we will need this to make pauses in between text and get a random color
color_list = ['magenta', 'red', 'yellow', 'blue', 'green', 'cyan', 'white']

def rainbow_text(x):
  for i in range(len(x)):
      random_color = random.choice(color_list)
      print(colored(x[i], random_color), end ="")
      time.sleep(0.04)
      sys.stdout.flush()
  print("")

while True:
  x = input("What word to you want to rainbow print?")
  rainbow_text(x)
