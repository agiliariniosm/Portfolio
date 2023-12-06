import random

options = ["rock", "fire", "ice"]
you_won = "\"You won fair and square. I release you from my lair. By the following decree, reunited you will be.\"\n૮ ˆﻌˆ ა"

def rock_fire_ice():
    print(f"\"Delightful {name}! If you win, I will give you your dog back and return both of you home."
          f"\nIf you loose, you will both stay here forever."
          f"\nReady set shoot!\"")
    while True:
        user_throw = input("\nThrow rock, fire, or ice: ").lower()
        random_number = random.randint(0,2)
        gnome_throw = options[random_number]
        if user_throw in options:
            print(f"The gnome threw {gnome_throw}")
        else:
            continue
        if user_throw == "rock" and gnome_throw == "fire":
            print(you_won)
            quit()
        elif user_throw == "fire" and gnome_throw == "ice":
            print(you_won)
            quit()
        elif user_throw == "ice" and gnome_throw == "rock":
            print(you_won)
            quit()
        elif user_throw == gnome_throw:
            continue
        else:
            print("You lost. You and your dog will stay forever in the gnome's meadow.")
            quit()


def snatch_foot():
    print("\nA hand comes out of the darkness, snatches your foot, and pulls you through a portal."
          "\nYou appear on a sunny meadow of flowers. The gnome stands before you with a devilish grin."
          f"\n\"I've been waiting for you {name}\" says the gnome.")
    answer_gnome = input("You a) scream, b) run away, c) wait for the gnome to speak again: ")
    if answer_gnome == "a":
        print("The gnome has a huge distaste for screams and sent you back to the beginning.")
    elif answer_gnome == "b":
        print("You will never out run the gnome. RIP.")
        quit()
    elif answer_gnome == "c":
        while answer_gnome == "c":
            print("The gnome speaks.\n\"Let's play rock, fire, ice. Rock beats fire, fire beats ice, and ice beats rock.")
            answer_play = input("Shall we play?\" ")
            if answer_play == "yes":
                rock_fire_ice()
                break
            else:
                print("The gnome only takes yes for an answer.")

print(
    "You are sitting at home coding when a gnome breaks into your room through the air vent and disappears with your dog."
    "\nWould you like to chase the gnome and save your dog?")
play_game = input("Type yes or no: ").lower()

if play_game == "yes":
    print("You have chosen to embark on an adventure.")
    name = input("What name will you use on this quest? ")
else:
    print("Karma will get you. Have a good day.")
    quit()

while play_game == "yes":
    print(
        "You jump after the gnome into darkness. You slip on something and feel that you are falling."
        "\nDo you a) embrace for impact and curl into a ball, b) try to land on your toes, or c) grab on to the ledge sticking out of the wall?")
    answer_fall= input("Type a, b, or c: ").lower()
    if answer_fall == "a":
        print("You chose the wrong way to fall from heights. Try again.")
    elif answer_fall == "b":
        print(
            "You knew how to soften your fall. Luckily the fall wasn't too high and a pile of leaves was waiting for you.")
        snatch_foot()
        break
    elif answer_fall == "c":
        print(
            "You grab on to the ledge and pull yourself up. The days you spent bouldering paid off and you're able to climb out of the vent."
            "\nHowever, you saved only yourself and your dog remains hostage.")
        answer_go_down = input("Would you like you like to go back down? ").lower()
        if answer_go_down == "yes":
            snatch_foot()
            break
        else:
            print("The gnomes grew bold and you were next. Karma got you.")
            break
    else:
        print("You don't know the rules, you loose.")
        break
