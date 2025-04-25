# Results for different prompt engineering techniques:

# PROMPT 1: Password Entropy Calculation
## Zero Shot

Model Response: To calculate the entropy of a 12-character password, we need to calculate the number of possible combinations.

* Uppercase letters: 26 possibilities

* Lowercase letters: 26 possibilities

* Digits: 10 possibilities

Total number of possible characters: 26 + 26 + 10 = 62

Since each character can be chosen independently, the total number of possible combinations is:
62^12 = 1,208,925,819,614,629,174,706

Time Taken: 5.844s

Result: Correct.

* The formula used and the steps taken to calculate the entropy are correct. The total number of possible characters is 62, and the explanation is accurate.


## Few-Shot

Time Taken: 5.831s

Result: Incorrect.


## Chain-of-Thought

Model Response:

* Step 1: We know the formula for entropy is:
Entropy = Length of password * log₂(number of possible characters)

* Step 2: Substitute the values:
Length of password = 12
Number of possible characters = 62 (26 uppercase + 26 lowercase + 10 digits)

* Step 3: Calculate the entropy:
Entropy ≈ 12 * log₂(62) ≈ 12 * 5.91 ≈ 70.29

Time Taken: 2.767s

Result: Correct.

* The formula and steps are accurate. The final entropy value of 70.29 bits is correctly calculated.

## Prompt Template

Model Response: 8.9872

Time Taken: 2.486s

Result: Incorrect.

* The calculated entropy value is incorrect. The correct value for a 12-character password using uppercase, lowercase letters, and digits should be closer to 70.29 bits (as shown in the other results). This output likely reflects an issue with how the prompt was handled.


## Generate Knowledge

Model Response (Generated Knowledge): To calculate the entropy of a 12-character password using uppercase, lowercase letters, and digits, we need to consider several factors.

Background Knowledge:

1. Character Set: The character set used in this problem includes:

* Uppercase letters (A-Z)

* Lowercase letters (a-z)

* Digits (0-9)

The total number of characters in the character set is 62 (26 uppercase + 26 lowercase + 10 digits).

2. Password Requirements: The password has a length of 12 characters, which means we have 12 positions to fill.

3. Entropy Calculation: Entropy is a measure of randomness or uncertainty in a system. In this case, it represents the unpredictability of the password.

Final Answer: To calculate the entropy of a 12-character password, we can use the formula:
Entropy (in bits) = Length of password * Log2(possible characters)


Time Taken: 11.472s

Result: Correct.



# PROMPT 2: Cyberattack Classification

## Zero Shot (Correct)

Output:
The type of cyberattack you've described is classified as a:
Distributed Denial-of-Service (DDoS) attack.
In a DDoS attack, the attacker uses multiple compromised devices (bots or zombies) to flood a targeted server or network with traffic, rendering it unavailable to legitimate users.

Time taken: 26.808s

## Few Shot (Correct)

Based on your description, I would classify this as:
Distributed Denial of Service (DDoS) – a type of cyberattack where an attacker floods a server or network with excessive traffic from multiple sources in order to make it unavailable or disrupt its operation.

Time taken: 6.384s

## Chain of Thought (Correct)

That's partially correct. While the description matches a Denial of Service (DoS) attack, it actually refers to a Distributed Denial of Service (DDoS) attack.
A DDoS attack is a coordinated assault that overloads a system’s resources using many compromised devices (botnets), causing denial of service.

Time taken: 9.684s

## Prompt Template (Incorrect)
Denial of Service (DoS) Attack
(Does not mention “Distributed” or use botnets, so it misses the key feature.)

Time taken: 3.148s


## Generate Knowledge (Correct)

Generated Knowledge Summary:

* Type of Attack: Distributed Denial-of-Service (DDoS)

* Definition: Overwhelming a system with traffic from multiple sources (botnets).

* How it Works: Uses zombies/botnets to flood a server and exhaust its resources.

Final Output:
This is clearly a DDoS attack.
Answer: Yes

Total Time Taken: 24.46s


# PROMPT 3: Access Control Model Identification

## Zero Shot (Correct)

The access control model described is known as a Role-Based Access Control (RBAC) model.

In RBAC, permissions are granted to users based on their roles within an organization, rather than their individual identities. This makes it flexible and scalable.

Time taken: 12.636s

## Few Shot (Correct)

Role-Based Access Control (RBAC)

Time taken: 3.054s

## Chain of Thought (Correct)

That's correct. The system model can be classified as Role-Based Access Control (RBAC) because:

1. Roles determine access rights

2. Access is based on roles rather than individual users or resources.

This setup ensures users gain permissions based on their assigned organizational role.

Time taken: 9.658s


## Prompt Template (Correct)

Role-Based Access Control (RBAC)

Time taken: 2.993s


## Generate Knowledge (Correct)
Generated Knowledge Summary:

The scenario indicates that permissions are assigned according to predefined user roles (e.g., manager, employee), matching the definition of RBAC.

Final Classification:
Role-Based Access Control (RBAC)

Reasoning:

* Permissions are granted based on organizational roles

* This is a core characteristic of RBAC

Total Time Taken: 26.971s
