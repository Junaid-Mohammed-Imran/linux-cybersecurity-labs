Day 12 — File & Permission Security

📌 Topics Covered

Topic 1 — File Permissions

- Learned the meaning of Linux file permissions:
  - "r" — Read
  - "w" — Write
  - "x" — Execute
- Learned about owner, group, and others.
- Used "ls -l" to view file permissions.

Topic 2 — File Ownership

- Learned that every file has an owner and an associated group.
- Used "ls -l /" to inspect file ownership.
- Identified the owner and group in the command output.

Topic 3 — "chmod"

- Learned that "chmod" changes file permissions.
- Created a test file named "testfile.txt".
- Checked its original permissions.
- Changed its permissions using "chmod 600".

touch testfile.txt
ls -l testfile.txt
chmod 600 testfile.txt
ls -l testfile.txt

Result: "-rw-------"

- Owner: Read and write
- Group: No permissions
- Others: No permissions

Topic 4 — "chown"

- Learned that "chown" changes file ownership.
- Checked the owner and group of "testfile.txt".
- Observed that both the owner and group were "root".

ls -l testfile.txt

Topic 5 — Security Implications

- Learned how incorrect permissions can expose sensitive files.
- Understood the risks of unauthorized reading and modification.
- Learned why correct ownership and minimum necessary permissions are important.

🛠️ Commands Practiced

ls -l
ls -l /
touch testfile.txt
chmod 600 testfile.txt
ls -l testfile.txt

🎯 What I Learned

- How to inspect Linux file permissions.
- How to identify file owners and groups.
- How to change permissions using "chmod".
- How file ownership works with "chown".
- How incorrect permissions can create security risks.

📅 Day

Day 12 of my Cybersecurity Learning Roadmap.

Status: ✅ Completed
