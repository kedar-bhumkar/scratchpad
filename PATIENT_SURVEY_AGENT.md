# Patient Survey Agent

Part of the scratchpad Salesforce project for managing patient appointments and surveys.

## Custom Objects

### Appointment__c
Custom object to track patient appointments.

**Fields:**
- **Name:** Appointment Number (Auto-Number: APT-{0000})
- **Appointment_Type__c** (Picklist)
  - Clinical Appointment
  - Non-Clinical Appointment
- **Contact__c** (Lookup to Contact)
  - Relationship: Appointments
  - Delete Constraint: Set Null

**Features:**
- Activities enabled
- History tracking enabled
- Reports enabled
- Sharing Model: Read/Write

## Deployment

```bash
# Deploy Appointment object
sf project deploy start --target-org my-research-org -d force-app/main/default/objects/Appointment__c
```

## Project Status

- ✅ Appointment custom object created
- ✅ Appointment Type picklist field
- ✅ Contact lookup field
