# Answers to Part 3

Add your answers to the questions in Part 3, Step 2 below. 

## Vulernability Remediation:
### Vulnerability 1: 
1. Which package or library are you addressing?
    Cryptography
2. Which CVE is linked to this vulnerability?
    CVE-2024-0727
3. What remediation steps do you suggest?
    We can upgrade cryptography package from 39.0.1 to the latest version (42.0.2). We can also ensure that the python dependencies are pinned to secure verions with the requirements file. Also, we can rebuild and redeploy the application image after the dependency update to verify no residual vulnerablities. Lastly, we can run a new static and image scan to confirm.

### Vulnerability 2:
1. Which vulnerability are you addressing?
    Pillow
2. Which CVE is linked to this vulnerability?
    CVE-2024-28219
3. What remediation steps do you suggest? 
    We can upgrade Pillow library from 9.4.0 to the latest version (10.3.0). We can review any custom image-processing logic that may be infected. We can also test the upgraded application package to check backwards compatibility. Lastly, we can perform a follow up scan to verify if the CVE alert is still triggered.