# Black Box

### AI agents do the work. Black Box keeps them accountable.

A hackathon prototype by **Saeid Hashim**.

Give an agent clear boundaries. Watch its work. Keep the blocked attempts in the record. Let a human make the final decision.

![Black Box overview](https://github.com/user-attachments/assets/d50a005f-de0f-4d3c-a8f8-806935c7532b)

## Try it

[Open the live Black Box app](https://saeidhashim.github.io/black-box/) in your browser.

Or run it offline:

1. Download this repository using **Code → Download ZIP**.
2. Extract the ZIP and open **index.html** in a modern browser.
3. Open **Agents**, choose an issue, and follow the five stages.
4. Select an employee and enter the demo password **1234** to sign off.

No install, build step, API key, or internet connection is needed to run the app. The app is a single HTML file.

## One issue. Five stages.

| Stage | What happens |
| --- | --- |
| **Warrant** | Define what the agent may do, what it must never do, and how long its permission lasts. |
| **Investigate** | Read simulated evidence, check recent changes, and trace the cause. |
| **Enforce limits** | Block prohibited actions and pause a service restart for human approval. |
| **Review** | Check the record chain, inspect the flagged attempt, and read the recommendation. |
| **Sign off** | Choose the initiating employee and record the final human decision. |

The stage bar and timer stay visible as the incident moves forward. Earlier stages remain available, and the header shifts from white to black as work progresses.

## Built for a clear handoff

- **Five scenarios:** payment failure, sign-in timeouts, inventory mismatch, stuck notifications, and slow search.
- **Visible boundaries:** each agent has its own goal, allowed actions, and prohibited actions.
- **A complete record:** actions and blocked attempts enter a linked SHA-256 record chain.
- **Human control:** risky repairs wait for approval. Sign-off records the selected employee.
- **Records and Reviews:** revisit saved incidents, inspect evidence, and export the record as JSON.
- **Offline PDF brief:** a two-page summary explains the cause, repair, blocked action, outcome, and sign-off status.

![Employee sign-off](https://github.com/user-attachments/assets/6bbcbdf9-10d6-4544-87bf-39f7882b969e)

## What this prototype does not claim

Black Box is an **offline simulation**, not a live incident-response system. It does not connect to an AI model, production services, or real customer data. Service changes and recovery metrics are scenario data.

The record chain is a local integrity check, not independent proof that real-world actions occurred. The shared password **1234** is a demo check, not secure employee authentication. Selecting a name does not verify that person's identity.

Saved incident records stay in the current browser's local storage. Browser settings or clearing site data can remove them. There is no server or account sync.

## Files

```text
index.html                 Self-contained offline app
```

The interface uses HTML, CSS, and JavaScript with no external libraries or network assets. 
