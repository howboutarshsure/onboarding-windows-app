# Code Signing & Deployment Process

## ❓ Why is this important?

Code signing is a vital security step in software development. It ensures that the application hasn’t been tampered with and confirms the identity of the publisher. Even though someone else may manage the signing (e.g., Manish), understanding the process is important for ensuring secure and trustworthy deployments.

## 🔍 Research & Learn

### What is code signing and how does it secure applications?

Code signing uses a digital certificate to sign application code. This signature validates the origin and integrity of the application. If the code is modified after being signed, the signature becomes invalid, alerting the user to potential tampering.

### How does Azure Code Sign with an EV certificate work?

Azure Code Sign with an EV (Extended Validation) certificate provides a highly trusted level of verification. EV certificates require strict validation of the publisher’s identity and are stored in secure hardware (HSM). Applications signed with EV certificates show fewer warning prompts in Windows, improving user trust and installation success rates.

### What are the broader implications of the deployment process?

A secure deployment process ensures that applications reach users safely and work reliably. Steps like code signing, integrity checks, and environment validation reduce the risk of malware injection, corrupted files, or deployment errors. It also improves user confidence and the overall reputation of the product.

## 📝 Reflection

### Why is code signing a critical step in the deployment process?

It proves that the code is authentic and hasn’t been altered. Without it, users might see security warnings, or worse, unknowingly run tampered or malicious code. It builds a bridge of trust between developers and users.

### How does understanding the deployment process impact your approach to development?

Knowing how the final product is packaged, verified, and delivered makes me more careful with dependencies, updates, and testing. It helps me think beyond just writing code — I consider how it will be used and trusted by end users.

### What risks could arise if code signing is overlooked or improperly managed?

- Users may see security warnings or installation may be blocked.
- Software could be altered without detection.
- Loss of user trust and potential brand damage.
- Increased exposure to malware risks.

## 🛠️ Task

### Summary of Insights

- Code signing is essential for protecting software integrity and authenticity.
- Azure Code Sign with EV certificates enhances user trust and reduces friction during installation.
- Developers should understand the deployment flow to build secure, production-ready applications.

## 📄 Saved as: code-signing-reflection.md
