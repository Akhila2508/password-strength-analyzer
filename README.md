# password-strength-analyzer
# Password Strength Analyzer

A simple Python tool that checks how strong a password is and suggests ways to improve it.

## What it does

The script asks the user to enter a password, then checks it against five criteria:

- **Length** — rewards passwords of 8+ characters, and more for 12+ characters
- **Uppercase letters** — checks for at least one A–Z character
- **Lowercase letters** — checks for at least one a–z character
- **Numbers** — checks for at least one digit
- **Special characters** — checks for symbols like `! @ # $ % ^ & *`

Each check that passes adds to a score. Based on the total score, the password is rated:

- **Weak** (score 0–3)
- **Medium** (score 4–5)
- **Strong** (score 6+)

If any checks fail, the tool prints specific suggestions — for example, "Add uppercase letters" — so the user knows exactly how to improve their password.

## How to run it

1. Make sure Python 3 is installed.
2. Run the script from a terminal:

   ```
   python3 password_analyzer.py
   ```

3. Enter a password when prompted.
4. The tool prints the strength rating and any suggestions for improvement.

## Example

```
Enter your password: test123

Password Strength: Weak

Suggestions:
- Increase password length to at least 12 characters.
- Add uppercase letters.
- Add special characters.
```

## Why this matters

Many real-world data breaches happen because of weak, reused, or easily guessed passwords. This tool demonstrates basic principles of password security — length, character variety, and complexity — that make passwords significantly harder to crack.

## Possible future improvements

- Check entered passwords against a list of commonly breached passwords
- Store hashes of previously used passwords to detect and prevent reuse
- Build a simple web interface so the tool can be used without a terminal
