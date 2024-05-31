 Process for the following secure manual code review 
 Identify Security-Sensitive Areas:

User input (username and password)
User authentication (checking username and password)
Review User Input:

Vulnerability: The code doesn't validate or sanitize user input. An attacker could enter malicious code disguised as a username or password.
Recommendation: Implement input validation to restrict characters allowed in the username and password. Consider using libraries for more advanced validation.
Review User Authentication:

Vulnerability: Passwords are stored in plain text within the code. This is a major security risk if the code is compromised.
Recommendation: Never store passwords in plain text. Use a secure hashing algorithm (like bcrypt) to store one-way hashes of passwords.

Session Management: This simple example doesn't implement session management. In a real application, consider using secure session tokens to maintain user login state.
Error Handling: The code doesn't handle potential errors, like a user entering a non-existent username. Implement robust error handling to prevent unexpected behavior.

These are all the steps for manual code reviewing for simple login system.
