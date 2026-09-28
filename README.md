# 🔐 SentinelMDM — Lock Confirmation

> **Secure. Manage. Monitor. Comply.**

A modern **Mobile Device Management (MDM)** interface concept designed for Android fleet administration. This repository showcases the **Remote Lock Confirmation** experience within the SentinelMDM Device Detail workflow.

---

## 📱 Screen Preview

### Remote Lock Confirmation

The Lock Confirmation screen appears when an administrator attempts to remotely lock a managed device.

It provides a clear confirmation step before the action is executed while giving the administrator useful information about the effect of the lock.

---

## ✨ Key Features

### 🔒 Remote Device Lock

Administrators can initiate a remote lock for a managed Android device from the Device Detail screen.

**Example target:**

```text
Pixel 8 Pro (Alex Chen)
```

---

### 📝 Custom Lock-Screen Message

Administrators can enter a custom message that can be displayed on the device's lock screen.

Example:

> This device is managed by Campus IT. Please return to Tech Support Desk, Hall B.

The interface includes a **120-character limit** with a real-time character counter.

```text
74 / 120
```

---

### 🚨 Emergency Dialer Indicator

The interface clearly communicates that emergency calling remains available after the device is locked.

```text
● Emergency dialer stays enabled
```

This helps prevent administrators from confusing a remote lock with a destructive device action.

---

### 🛡️ Zero Data Loss Information

A dedicated safety information panel explains that locking the device does **not represent a factory reset or data-wiping operation**.

```text
Zero Data Loss

Cloud backups and ongoing academic sync operations
will safely continue in the background.
```

---

### 🎯 Clear Action Hierarchy

The interface uses two primary actions:

| Action          | Purpose                                 |
| --------------- | --------------------------------------- |
| 🔒 Confirm Lock | Continue with the remote lock operation |
| Cancel          | Dismiss the confirmation sheet          |

The confirmation button uses a large touch target suitable for mobile interaction.

---

## 🎨 UI Design

The interface follows a dark, modern administrative-console aesthetic.

### Design Tokens

| Token          | Value     |
| -------------- | --------- |
| Background     | `#0B0C10` |
| Surface        | `#121318` |
| Card           | `#1A1B21` |
| Border         | `#272932` |
| Input          | `#0F1015` |
| Primary Action | `#F59E0B` |
| Success        | `#10B981` |
| Information    | `#3B82F6` |

### Typography

**Plus Jakarta Sans**

The typography is used to maintain a clean and modern administrative UI appearance.

### Icons

**Lucide Icons**

Used for:

* 🔒 Lock
* 🛡️ Shield
* 🛡️ Shield Check
* ← Back
* ⋮ More Actions

---

## 🧩 User Flow

```text
Device Inventory
       │
       ▼
Device Detail
       │
       ▼
Device Actions
       │
       ▼
Remote Lock
       │
       ▼
┌──────────────────────────────┐
│   Lock Device Remotely       │
│                              │
│   Target Device              │
│   Pixel 8 Pro                │
│                              │
│   Lock Screen Message        │
│   ┌──────────────────────┐   │
│   │ Custom message...    │   │
│   └──────────────────────┘   │
│                              │
│   ● Emergency dialer        │
│     stays enabled            │
│                              │
│   🛡 Zero Data Loss          │
│                              │
│   [   🔒 Confirm Lock   ]    │
│   [       Cancel        ]    │
└──────────────────────────────┘
```

---

## 🛠️ Technologies Used

* **HTML5**
* **Tailwind CSS**
* **JavaScript**
* **Lucide Icons**
* **Plus Jakarta Sans**
* Responsive Mobile UI
* Dark UI Design

---

## 📂 Project Structure

```text
SentinelMDM/
│
├── lock-confirmation.html
│
├── README.md
│
└── assets/
    └── screenshots/
        └── lock-confirmation.png
```

---

## 🚀 Run Locally

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/SentinelMDM.git
```

Open the project:

```bash
cd SentinelMDM
```

Then open:

```text
lock-confirmation.html
```

in your browser.

No build system or package installation is required for this prototype.

---

## 🌐 GitHub Pages

This screen can also be hosted using **GitHub Pages**.

After enabling GitHub Pages, the screen can be accessed using:

```text
https://YOUR-USERNAME.github.io/SentinelMDM/lock-confirmation.html
```

---

## 🧪 Current Prototype Behavior

This project currently focuses on **UI/UX demonstration**.

### Implemented

* ✅ Mobile device frame
* ✅ Bottom-sheet modal
* ✅ Remote lock confirmation
* ✅ Custom lock-screen message
* ✅ Character counter
* ✅ 120-character validation
* ✅ Emergency dialer indicator
* ✅ Zero-data-loss information
* ✅ Confirm Lock interaction
* ✅ Cancel interaction
* ✅ Escape-key dismissal
* ✅ Responsive layout
* ✅ Dark theme

### Planned

* ⬜ Backend API integration
* ⬜ Device authentication
* ⬜ Device status synchronization
* ⬜ Real Android Device App communication
* ⬜ Lock command delivery
* ⬜ Command execution history
* ⬜ Lock status confirmation
* ⬜ Audit logs

---

## 🔐 Important Note

This repository is an **academic and internship demonstration project**.

The current implementation demonstrates the **administrator-side UI/UX and interaction flow**.

The `Confirm Lock` action currently simulates a remote lock operation and does not independently lock a physical Android device.

---

## 🎯 Project Goal

SentinelMDM aims to explore how a simplified MDM platform can provide administrators with a clear interface for managing managed devices.

The design focuses on:

* **Simplicity**
* **Clarity**
* **Safe administrator actions**
* **Mobile-first interaction**
* **Transparent device controls**
* **Clean enterprise UI**

---

## 👨‍💻 Author

**Kartikey Vishwakarma**

B.Tech — Information Technology
Dr. Ram Manohar Lohia Avadh University
Institute of Engineering and Technology, Ayodhya

---

## ⭐ Project Status

```text
Status: 🚧 Active Development

UI/UX Prototype:     ✅
Frontend Demo:       ✅
Backend Integration: 🚧
Android Integration: 🚧
Production MDM:      ❌
```

---

## 📌 Disclaimer

SentinelMDM is developed for **educational, academic, UI/UX, and internship demonstration purposes**.

It is not intended to replace production-grade enterprise MDM solutions or Android Enterprise management infrastructure.

---

### ⭐ If you find this project useful, consider starring the repository!
