#!/usr/bin/env python3
import time
import sys

def prank_countdown(seconds):
    """Display a fake countdown warning of a system meltdown."""
    for sec in range(seconds, 0, -1):
        # The \r carriage return brings the cursor to the start of the line.
        sys.stdout.write(f"\rWARNING: System meltdown in {sec} seconds...")
        sys.stdout.flush()
        time.sleep(1)
    # Erase the warning and display the prank message.
    sys.stdout.write("\rAPRIL FOOLS! Your system is completely safe.      \n")
    sys.stdout.flush()

def main():
    print("Initializing system check...\n")
    time.sleep(2)  # Pause for dramatic effect.
    
    # Start the fake countdown (e.g., countdown from 10 seconds)
    prank_countdown(10)
    
    time.sleep(1)
    print("\nHappy April Fools' Day!\nEnjoy the joke.\n")

if __name__ == "__main__":
    main()
