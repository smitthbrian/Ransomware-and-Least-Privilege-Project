# Ransomware and Least Privilege 🔒

**Course:** Ethical Hacking & Countermeasures  
**Author:** Brian F. Smith  

This project focuses on the critical concepts of ransomware defense and the Principle of Least Privilege (PoLP). It demonstrates how to secure file-sharing environments in Windows Server to reduce the spread of ransomware, using user account and group-based permission management. To see the work achieved in this project, browse the .pptx file attached to the main branch.

---

## 📁 Project Overview

### What is Ransomware?  
Ransomware is a type of malware that encrypts files and demands ransom for decryption. It often spreads via phishing emails, compromised software, or vulnerable systems. Shared folders are frequent ransomware targets due to their wide access and insufficient permission controls.

### What is the Principle of Least Privilege (PoLP)?  
The Principle of Least Privilege ensures users and processes only have access to the files and directories they need. Implementing PoLP can significantly reduce vulnerability to ransomware attacks by limiting file access and the potential spread of malware.

---

## 🔧 Project Steps and Configuration

1. **Setting Up File Sharing in Windows Server**  
   - Created user accounts in Active Directory for Jane and John Doe.  
   - Configured a shared folder named "CIS" with role-based permissions.

2. **Group Creation and Permission Management**  
   - Created a "CIS" group in Windows Server and assigned Jane and John as members.  
   - Configured NTFS and share permissions to allow "Change" and "Read" access for the group.

3. **Connecting to the Shared Folder**  
   - Verified folder access from a client machine using assigned credentials.  
   - Ensured firewall settings and file-sharing rules were enabled.

---

## 🔍 Folder Permissions and Use Cases

### Use Case 1: Document Creation and Read Access  
- **Permissions Assigned:** "Modify" or "Change" for document creators; "Read" for others.  
- **Security Benefit:** Document creators retain control, while others can view without modifying.

### Use Case 2: Editing Existing Documents  
- **Permissions Assigned:** "Change" for users needing edit rights.  
- **Security Benefit:** Enables collaborative editing without altering folder security.

### Use Case 3: Collaborative Document Creation  
- **Permissions Assigned:** "Change" or "Modify" for group collaboration.  
- **Security Benefit:** Facilitates teamwork while mitigating unauthorized permission changes.

---

## 🛡️ RanSim Demonstration: Ransomware Effects

A simulated ransomware attack using RanSim.ps1 demonstrated how different permissions affect file encryption:  
- **Full Control:** All files were encrypted.  
- **Read Only:** Minimal or no files were affected.

---

## 📋 Best Practices for Ransomware Defense

1. **Implement Least Privilege:** Assign only the necessary permissions for users' tasks.  
2. **Regularly Audit Permissions:** Conduct periodic reviews to align permissions with job roles.  
3. **Enable Multi-Factor Authentication (MFA):** Adds a critical layer of protection.  
4. **Maintain Offline Backups:** Ensure regular, secure backups are available.  
5. **Simulate Ransomware Attacks:** Test recovery procedures and team readiness.

---

## 🎯 Conclusion

This project highlights the importance of proper permission management and ransomware defense. By applying PoLP and best practices, organizations can reduce vulnerability to attacks while maintaining smooth collaboration.

---

## 🌱 Connect With Me

[<img align="left" alt="Brian Smith | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/linkedin.svg" />][linkedin]

[linkedin]: https://www.linkedin.com/in/briansmith2025/
