# CIA-in-Cloud-Using-Block-Chain-Technology


## Installation Instructions for Truffle and Ganache

### Install Node.js

1. **Node.js and npm Installation:**
   - Ensure Node.js version 14 to 18 is installed. Use a Node Version Manager (NVM) to avoid permission errors:
     - For example, on OSX or Linux, install Node.js v18 using `nvm install 18`.
     - Confirm the installation by running `node --version`.

### Install Truffle

2. **Install Truffle:**
   - Open a terminal and use npm to install Truffle (avoid using `sudo` to prevent permission errors):
     ```bash
     npm install -g truffle
     ```
   - Confirm the installation by running:
     ```bash
     truffle version
     ```

### Install Ganache

3. **Install Ganache:**
   - Visit the [Ganache Releases Page] (https://github.com/trufflesuite/ganache-ui/releases).
   - Download the Ganache version suitable for your operating system.
   - Follow the installation instructions for your OS.

4. **Confirm Ganache Installation:**
   - After installation, open Ganache to ensure it launches without errors.

Now you have Truffle and Ganache installed, essential tools for Ethereum development and smart contract testing.

## Contract Initialization Algorithm (Python)

```python
def initialize_contract(Identifier, Policy, View, Signature):
    if Identifier not in ["Stakeholder", "Owner"]:
        return "Invalid parties"
    
    Nodeid = generate_node_id(Policy, Dataid)
    Attachment = combine_contract_data(Contract, Datacurrent)
    Helper = translate_attachment_to_control(Attachment)
    Access(Helper, Stakeholderid)
    return "Initialized contract code"

def generate_node_id(Policy, Dataid):
    # Implement your logic here
    pass

def combine_contract_data(Contract, Datacurrent):
    # Implement your logic here
    pass

def translate_attachment_to_control(Attachment):
    # Implement your logic here
    pass

def Access(Helper, Stakeholderid):
    # Implement your logic here
    pass

result = initialize_contract("Stakeholder", "PolicyData", "DataCurrent", "OwnerSignature")
print(result)
```

## Access Control Algorithm (Java)

```java
public class Access {
    public static void main(String[] args) {
        String Identifier = "Stakeholder";
        String Validate = "Contract";
        HashMap<String, String> Mapping = new HashMap<>();
        Mapping.put("Data", "Owner");
        String result = accessContract(Identifier, Validate, Mapping);
        System.out.println("Access contract code: " + result);
    }

    public static String accessContract(String Identifier, String Validate, HashMap<String, String> Mapping) {
        String Action = "Write";
        if (Action.equals("Write")) {
            String Stakeholder = "Apply modification";
            String Timestamp = "Record(Timestamp)";
            String Modificationsig = "Signature";
            sendModificationsigToOwner(Modificationsig);
            return Stakeholder + "\n" + Timestamp + "\n" + Modificationsig;
        } else {
            String Modificationsig = "Receive: Modificationsig ← Owner";
            validateModificationsig(Modificationsig);
            String Transcript = "Transcript → Computing Node";
            String Timestamp = "Record(Timestamp)";
            return Modificationsig + "\n" + Transcript + "\n" + Timestamp;
        }
    }

    public static void sendModificationsigToOwner(String modificationsig) {
        System.out.println("Send: " + modificationsig + " → Owner (provenance)");
    }

    public static void validateModificationsig(String modificationsig) {
        System.out.println("Validate: " + modificationsig + " ← Owner");
    }
}
```

## Action Contract Algorithm (Java)

```java
public class MonitorActionContract {

    public static void main(String[] args) {
        String Identifier = "Stakeholder";
        String Policy = "PolicyData";
        String Datacurrent = "DataCurrent";
        String result = monitorActionContract(Identifier, Policy, Datacurrent);
        System.out.println("Monitor action contract code: " + result);
    }

    public static String monitorActionContract(String Identifier, String Policy, String Datacurrent) {
        String Action = "Read";
        if (!Policy.contains(Action)) {
            return "Revoke Access";
        } else {
            return "Grant Access";
        }
    }
}
```

