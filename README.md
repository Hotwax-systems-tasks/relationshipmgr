# Relationship Manager (relationshipmgr)

This project implements a Party Data Model using the Moqui framework to manage organizations, individuals, their roles, and contact mechanisms.

## Features
- **Party Management**: Supports both `Person` and `Organization`.
- **Role Management**: Assign roles like `Customer`, `Employee`, and `Employer` to parties.
- **Contact Mechanisms**: Stores postal addresses, phone numbers, and emails.
- **User Interface**: Forms and screens to manage and display party data.
- **Real-Life Data**: Uses sample data from a college setup (students, teachers, departments).

## Setup
1. Clone the repository.
2. Add the component to your Moqui instance.
3. Load seed data using provided JSON.
4. Access the UI to manage parties and contacts.

## Example Data
### Person
```json
{
  "Party": {
    "partyId": "PER123",
    "partyTypeId": "PERSON",
    "Person": {
      "firstName": "John",
      "lastName": "Doe",
      "birthDate": "1990-01-01"
    },
    "PartyRole": [
      { "roleTypeId": "CUSTOMER" },
      { "roleTypeId": "EMPLOYEE" }
    ]
  }
}
```

### Organization
```json
{
  "Party": {
    "partyId": "ORG456",
    "partyTypeId": "ORGANIZATION",
    "Organization": {
      "organizationName": "ABC"
    },
    "PartyRole": {
      "roleTypeId": "EMPLOYER"
    }
  }
}
```

## Usage
- View and manage people and organizations.
- Assign roles and contact mechanisms.
- Demonstrate party relationships using real-life examples.

