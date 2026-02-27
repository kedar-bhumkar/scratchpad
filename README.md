# Scratchpad - Salesforce Project

A Salesforce DX project for quick experiments and deployments.

## Project Structure

```
scratchpad/
├── sfdx-project.json
├── force-app/main/default/
│   └── objects/
│       └── Contact/
│           └── fields/
│               └── User_Attribution__c.field-meta.xml
```

## Custom Fields

### Contact Object
- **User_Attribution__c** - Text field (255 characters) for user attribution data

## Deployment

```bash
sf project deploy start --target-org my-research-org
```
