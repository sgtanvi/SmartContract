# Frontend

1. user interface
- Show input field for Ethereum contact address
- "Check Status" button

2. handle on click ("Check Status")
- Capture user input (contact address)
- send POST request to backend /validate-contract with address
- while waiting: 
    - Show animation of spinner
- On success:
    - Display data:
        - (name, symbol, supply, paused, owner)
- On Error:
    - Show Error Message
        - invalid address

