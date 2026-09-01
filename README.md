# SOFTWARE ENGINEERING LAB – 1

## Requirements Engineering & UML Use-Case Modelling

### Problem Statement #14
### Corporate Mental Wellness & Counseling Platform

---

## STUDENT DETAILS

**NAME: NIRANJAN S**

**SRN: PES1UG24AM177**

**SOFTWARE ENGINEERING LAB TEAM: 14**

---

## 1. PROBLEM STATEMENT

### Corporate Mental Wellness & Counseling Platform

The system is an anonymous enterprise counseling portal that allows employees to assess stress levels, book confidential sessions with licensed therapists, and track personal wellness indicators without employer identity disclosure.

### Target Actors

- Corporate Employee
- Licensed Therapist

The platform focuses on confidentiality, anonymous access, counseling appointment management, and personal wellness tracking.

---

## 2. LAB OBJECTIVE

The objective of this laboratory exercise is to elicit and document functional and non-functional requirements from the given scenario and translate them into a UML use-case model.

The exercise covers:

- Requirements elicitation and documentation
- Functional and non-functional requirement identification
- Requirement prioritization
- Definition of measurable acceptance criteria
- Identification of system actors and use cases
- UML use-case modelling
- Use-case flow specification
- Identification of alternate flows and error conditions

---

## 3. REQUIREMENTS SPECIFICATION

The requirements specification consists of exactly five Functional Requirements and two Non-Functional Requirements.

### 3.1 Functional Requirements

| Req ID | Description |
|---|---|
| FR-001 | The system shall generate an anonymized pseudo-ID for employee accounts to book counseling sessions without revealing corporate email or employee ID to the therapist. |
| FR-002 | The system shall allow employees to assess their stress and wellness levels. |
| FR-003 | The system shall allow employees to book confidential counseling sessions with licensed therapists. |
| FR-004 | The system shall allow licensed therapists to manage their counseling appointments. |
| FR-005 | The system shall allow employees to track their personal wellness indicators. |

### 3.2 Non-Functional Requirements

| Req ID | Description |
|---|---|
| NFR-001 | The appointment scheduler must handle timezone conversions accurately across global office locations. |
| NFR-002 | The system shall protect employee identity and confidential counseling information from unauthorized disclosure. |

Each requirement is documented with its Requirement ID, Type, Description, Priority, Acceptance Criteria, and Rationale.

---

## 4. SYSTEM ACTORS

### 4.1 Corporate Employee

The Corporate Employee interacts with the system to:

- Assess stress and wellness levels
- Book confidential counseling sessions
- Track personal wellness indicators
- Access counseling services without unnecessary disclosure of corporate identity

### 4.2 Licensed Therapist

The Licensed Therapist interacts with the system to:

- Access counseling appointment information
- Manage scheduled appointments
- Conduct counseling sessions

### 4.3 Platform Administrator

The Platform Administrator performs administrative operations required for managing the platform.

---

## 5. UML USE-CASE MODEL

The UML use-case diagram models the interaction between the identified actors and the Corporate Mental Wellness & Counseling Platform.

### Primary Use Cases

- Assess Stress Level
- Book Counseling Session
- View Wellness Indicators
- Manage Appointments
- Generate Anonymous Pseudo-ID
- Authenticate User
- Select Therapist
- Cancel/Reschedule Session

### UML Relationships

The model includes both required UML relationship types.

**`«include»` Relationship**

The `«include»` relationship represents behaviour that is required as part of another use case.

Example:

`Book Counseling Session` `«include»` `Generate Anonymous Pseudo-ID`

**`«extend»` Relationship**

The `«extend»` relationship represents optional or conditional behaviour associated with a base use case.

Example:

`Cancel/Reschedule Session` `«extend»` `Book Counseling Session`

---

## 6. USE-CASE FLOW

### Use Case: Book Counseling Session

#### Preconditions

1. The employee has access to the platform.
2. The employee has completed the required authentication.
3. Therapist availability is available in the system.

#### Main Success Scenario

1. The employee opens the counseling section.
2. The system displays available counseling options.
3. The employee selects a preferred therapist, date, and time.
4. The system validates therapist availability.
5. The system generates or retrieves the employee's anonymous pseudo-ID.
6. The system confirms the appointment details.
7. The system records the counseling appointment.
8. The system displays the booking confirmation.
9. The use case ends successfully.

#### Alternate Flow

**Appointment Slot Unavailable**

1. The system informs the employee that the selected appointment slot is unavailable.
2. The system displays alternative available slots.
3. The employee selects another available slot.
4. The system validates the new selection.
5. The booking process continues from the confirmation stage.

---

## 7. PRIVACY CONSIDERATIONS

Anonymity and confidentiality are key aspects of the system.

The platform generates an anonymized pseudo-ID for employee accounts so that the therapist does not receive the employee's corporate email address or employee ID through booking metadata.

The intended interaction is:

```text
Employee Identity
       |
       v
Anonymous Pseudo-ID
       |
       v
Therapist Interface
```

This ensures that counseling sessions can be booked while minimizing unnecessary disclosure of employee identity.

---

## 8. DELIVERABLES

The following deliverables are included in the repository:

| No. | Deliverable | Status |
|---|---|---|
| 1 | Complete Requirements Table | Completed |
| 2 | Five Functional Requirements | Completed |
| 3 | Two Non-Functional Requirements | Completed |
| 4 | UML Use-Case Diagram | Completed |
| 5 | `«include»` Relationship | Included |
| 6 | `«extend»` Relationship | Included |
| 7 | Use-Case Flow Specification | Completed |
| 8 | Alternate Flow | Included |

---

## 9. REPOSITORY STRUCTURE

```text
Software-Engineering-Lab-1/
│
├── README.md
│
├── Requirements/
│   └── Lab1_Requirements_Table_Problem14.docx
│
├── UML/
│   └── Lab1_UML_Use_Case_Diagram_Problem14.pdf
│
└── Use-Case-Flow/
    └── Lab1_Use_Case_Flow_Problem14.pdf
```

---

## 10. REQUIREMENT VALIDATION

The requirements were evaluated based on the following criteria:

### Clarity

Each requirement specifies the intended system behaviour without unnecessary ambiguity.

### Testability

Each requirement contains measurable acceptance criteria that allow the requirement to be evaluated as Pass or Fail.

### Relevance

Each requirement is aligned with the Corporate Mental Wellness & Counseling Platform described in Problem Statement #14.

---

## 11. STUDENT INFORMATION

| Field | Details |
|---|---|
| **Name** | **NIRANJAN S** |
| **SRN** | **PES1UG24AM177** |
| **Software Engineering Lab Team** | **14** |
| **Problem Statement** | **#14 – Corporate Mental Wellness & Counseling Platform** |
| **Laboratory** | **Lab 1 – Requirements Engineering & UML Use-Case Modelling** |
| **Department** | **Department of Computer Science & Engineering** |
| **University** | **PES University** |

---

**Software Engineering Laboratory – Lab 1**

**Requirements Engineering & UML Use-Case Modelling**

**Problem Statement #14**
