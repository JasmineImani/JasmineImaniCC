<h1>Hi, I'm Jasmine, an <a href="https://www.linkedin.com/in/jasmine-duerson-27b43a264/">IT and Cybersecurity Professional</a>☺</h1>

<h2>👨‍💻 Information Technology Projects:</h2>

- <b>osTicket (Help Desk Ticketing System)</b>
  - [osTicket: Prerequisites and Installation](https://github.com/joshmadakorcc/osticket-prereqs)
  - [osTicket: Post-Installation Configuration](https://github.com/joshmadakorcc/post-install-config)
  - [osTicket: Ticket Lifecycle Examples](https://github.com/joshmadakorcc/ticket-lifecycle)
- <b>Microsoft Azure</b>
  - [Configuring On-premises Active Directory within Azure VMs](https://github.com/joshmadakorcc/configure-ad)
  - [Network Security Groups (NSGs) and Inspecting Network Protocols](https://github.com/joshmadakorcc/azure-network-protocols)
  - [Virtual Private Networks (VPNs)](www.google.com)

<h2>👨‍💻 Cybersecurity Projects:</h2>

- <b>Kali Linux</b>
  - [Kali Linux: Prerequisites and Installation](www.google.com)
  - [Kali Linux: Post-Installation Configuration](www.google.com)
  - [Kali Linux: Hardening](www.google.com)
- <b>Kali Linux (Encrypting and Decrypting File with Ccrypt)</b>
  - [Kali Linux: Ccrypt Installation](www.google.com)
  - [Kali Linux: Create And Encrypt A File](www.google.com)
  - [Kali Linux: Change The Encryption Key](www.google.com)
  - [Kali Linux: Decrypt The File](www.google.com)
- <b>OWASP ZAP (Penetration Testing)</b>
  - [OWASP ZAP: Prerequisites and Installation](www.google.com)
  - [OWASP ZAP: Test A Web Application](www.google.com)
  - [OWASP ZAP: Observe Test Results](www.google.com)
- <b>Python</b>
  - [Simple Game]

def print_board(board):
    for row in board:
        print(" | ".join(row))
        print("-" * 9)

def check_win(board, player):
    for row in board:
        if all(cell == player for cell in row):
            return True
    for col in range(3):
        if all(board[row][col] == player for row in range(3)):
            return True
    if all(board[i][i] == player for i in range(3)) or all(board[i][2 - i] == player for i in range(3)):
        return True
    return False

def main():
    board = [[" " for _ in range(3)] for _ in range(3)]
    current_player = "X"
    moves = 0

    while True:
        print_board(board)
        row = int(input(f"Player {current_player}, enter row (0, 1, or 2): "))
        col = int(input(f"Player {current_player}, enter column (0, 1, or 2): "))

        if board[row][col] == " ":
            board[row][col] = current_player
            moves += 1
            if check_win(board, current_player):
                print_board(board)
                print(f"Player {current_player} wins!")
                break
            elif moves == 9:
                print_board(board)
                print("It's a draw!")
                break
            current_player = "O" if current_player == "X" else "X"
        else:
            print("That spot is already taken. Try again.")

if __name__ == "__main__":
    main()
                                        
<h2>🤳Connect with me:</h2>


[<img align="left" alt="Josh | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />][linkedin]
[<img align="left" alt="Jasmine | Indeed" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/indeed.svg" />][indeed]

[indeed]: https://profile.indeed.com/?hl=en_US&co=US&from=gnav-menu-homepage&_ga=2.127246989.1420021767.1693766040-1858563378.1693766040
[linkedin]: https://www.linkedin.com/in/jasmine-duerson-27b43a264/
