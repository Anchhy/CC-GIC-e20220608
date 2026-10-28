# CC-GIC-e20220608

Cloud Computing (CC-GIC) lab submissions.

- **Student:** ET Anchhy
- **Student ID:** e20220608
- **Environment:** AWS Academy Learner Lab, Ubuntu

## Labs

| # | Topic | Folder | Status |
|---|-------|--------|--------|
| 1 | Amazon EC2 | [`lab1/`](./lab1) | Done |
| 2 | _TBA_ | `lab2/` | — |

## Repository structure

```
CC-GIC-e20220608/
├── README.md
├── lab1/
│   ├── README.md        # steps, commands, notes
│   └── screenshots/     # evidence of completed tasks
└── lab2/
```

## Lab 1 – Amazon EC2

**Goal:** Launch and connect to an EC2 instance in the AWS Academy Learner Lab.

**Steps**

1. Start the Learner Lab and open the AWS Console.
2. Launch an EC2 instance (Ubuntu AMI, `t2.micro` / `t3.micro`).
3. Create or select a key pair and download the `.pem` file.
4. Configure the security group to allow SSH (port 22).
5. Connect from Ubuntu:

   ```bash
   chmod 400 labsuser.pem
   ssh -i labsuser.pem ubuntu@<public-ip>
   ```

6. Verify the instance and capture screenshots.
7. Stop or terminate the instance when finished.

## Notes

- Credentials, key pairs (`*.pem`) and `.env` files are **not** committed. See `.gitignore`.
- Learner Lab sessions expire; instance public IPs may change after restarting the lab.