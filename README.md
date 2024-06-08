# Convert PEM to JKS

This GitHub Actions workflow executes the process of converting a PEM certificate file to a Java KeyStore (JKS) format and which can then be imported it into Salesforce. 

## Workflow Overview

1. **Convert PEM to P12**: The workflow converts the provided PEM certificate file to a PKCS12 format (.p12).
2. **Convert P12 to JKS**: The PKCS12 file is then converted to a Java KeyStore (.jks) format.

## Usage

1. **Create PEM File**: Provide the PEM file as a GitHub secret as: `PEM_FILE`.
2. **Set JKS Passphrase**: Provide the JKS passphrase as a GitHub secret as: `JKS_PASS`.
3. **Set JKS Alias**: Provide the JKS alias as a GitHub variable as: `JKS_ALIAS`.
4. **Run Workflow**: Trigger the workflow through the GitHub Actions UI or the CLI.
