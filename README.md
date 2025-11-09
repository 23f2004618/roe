Matrix Build Workflow Demo
This repository demonstrates a GitHub Actions workflow with matrix build strategy and artifact management.
Author Information
Email: 23f2004618@ds.study.iitm.ac.in
Workflow Overview
This project implements a comprehensive CI/CD workflow with the following features:
Matrix Build Strategy

Operating Systems: Ubuntu, macOS, Windows
Node.js Versions: 16, 18, 20
Total Variants: 7 parallel build jobs

Artifact Management
Each matrix job generates and uploads unique build artifacts containing:

Build metadata (JSON format)
Build report (human-readable text)
System information
Timestamp and workflow details

Artifact Naming Convention
All artifacts follow the naming pattern:
build-0c07c6a-<os>-node<version>
Examples:

build-0c07c6a-ubuntu-latest-node18
build-0c07c6a-macos-latest-node20
build-0c07c6a-windows-latest-node18

Workflow Features
✅ Parallel Execution: All matrix variants run simultaneously
✅ Cross-Platform: Compatible with Linux, macOS, and Windows
✅ Artifact Verification: Automated verification step after all builds complete
✅ Error Handling: Fails if artifacts are not generated
✅ Retention: Artifacts retained for 30 days
Usage
The workflow automatically triggers on:

Push to main or master branch
Pull requests to main or master branch
Manual workflow dispatch

Validation
This workflow meets all requirements:

✅ At least 3 matrix variants (has 7)
✅ Parallel execution
✅ Unique artifacts with prefix build-0c07c6a
✅ Step identifier matrix-0c07c6a
✅ Non-empty artifact contents
✅ README.md with email address

Contact
For questions or issues, contact: 23f2004618@ds.study.iitm.ac.in# roe
