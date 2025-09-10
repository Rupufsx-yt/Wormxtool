#!/usr/bin/env python3
import time
import sys

# ANSI color codes
RED = "\033[31m"
GREEN = "\033[32m"
YELLOW = "\033[33m"
BOLD = "\033[1m"
RESET = "\033[0m"

# Banner text
banner = f"""
██████╗  █████╗ ███████╗    ██████╗  ██████╗  ██████╗ ███████╗███╗   ███╗ ██╔══██╗██╔══██╗██╔════╝    ██╔══██╗██╔═══██╗██╔═══██╗██╔════╝████╗ ████║ ██████╔╝███████║█████╗      ██████╔╝██║   ██║██║   ██║█████╗  ██╔████╔██║ ██╔═══╝ ██╔══██║██╔══╝      ██╔══██╗██║   ██║██║   ██║██╔══╝  ██║╚██╔╝██║ ██║     ██║  ██║███████╗    ██████╔╝╚██████╔╝╚██████╔╝███████╗██║ ╚═╝ ██║ ╚═╝     ╚═╝  ╚═╝╚══════╝    ╚═════╝  ╚═════╝  ╚═════╝ ╚══════╝╚═╝     ╚═╝
"""

def progress_bar():
    for i in range(0, 101, 10):
        sys.stdout.write(f"\r{YELLOW}Progress: {i}%{RESET}")
        sys.stdout.flush()
        time.sleep(0.3)
    print()

def main():
    print(f"{RED}{BOLD}[!] SYSTEM BREACH TOOL INITIALIZING...{RESET}")
    time.sleep(1)
    progress_bar()
    print(f"{GREEN}[✓] Simulation completed{RESET}\n")
    print(f"{RED}{banner}{RESET}")
    print(f"{RED}{BOLD}🔴 YOUR SYSTEM IS HACKED 🔴{RESET}")

if __name__ == "__main__":
    main()
