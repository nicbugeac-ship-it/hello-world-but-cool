# -----------------------------------------
# My First GitHub Program
# A "Hello World" with personality
# -----------------------------------------

from colorama import Fore, Style, init
import pyfiglet

init(autoreset=True)

# This function prints a friendly greeting with neon effects.
def say_hello(name="world"):
    neon_color = Fore.CYAN + Style.BRIGHT
    
    # Big ASCII art for "HELLO"
    hello_art = pyfiglet.figlet_format("HELLO", font="slant")
    print(f"{neon_color}{hello_art}")
    
    message = f"Hello, {name}! 👋 I'm officially on GitHub!"
    print(f"{neon_color}{message}")
    print(f"{neon_color}🚀 Let's build something amazing together!")

    # Add a simple neon sign ASCII art
    print(f"{neon_color}   _______")
    print(f"{neon_color}  /       \\")
    print(f"{neon_color} |  GITHUB |")
    print(f"{neon_color}  \\_______/")

# Program entry point
if __name__ == "__main__":
    user_name = input("What's your name? ")
    say_hello(user_name)
