# User contact verification service

This service provides functionality of verification of user contacts such as email address or phone number
It simply creates a record with unique identifier(uuid4) to track the verification process.
Service generates random 6-digit code, associate it with an ID and save to database.
When you pass id of verification process and code it will try to match it. If code matches - verified.

### Build & Run

```bash
docker-compose up --build -d
```

### Stop Everything

```bash
docker-compose down
```

## Contribute

This package is for use in some of my projects but everyone is welcome to submit a pull-request