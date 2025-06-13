# 📄 Use Case: User register

## 🎭 Primary Actor
- Guest

## 🎯 Goal
- Allow user to register in the platform.

## ✅ Preconditions
- The user must not be registered previously.
- Required data  fields must be filled with valid inputs.
 
## 🔄 Main Flow
1. The user accesses to the sing up section.
2. The user fill the data fields.
3. The user press the register button.
4. The system checks the user data.
5. The system save the user data at PostgreSQL.
6. Confirmation about the register.

## 🔁 Alternative Flows
- **Invalid data user**  
  The system shows a message with the invalid inputs.
- **Existent user**  
  The system shows a message informing to the user.

## 🧾 Postcondiciones
- A new user account is created in the system and stored in PostgreSQL.
- The user can now log in using the registered credentials.

## ⚠️ Reglas de Negocio Relacionadas
- Name length: 5, 50
- Last name length: 5, 50
- Password: 8 chars, 1 Lower, 1 Capital letter, 1 Number
- Email: Unique and valid format

## 📌 Notas Técnicas
- The password must send always encrypted