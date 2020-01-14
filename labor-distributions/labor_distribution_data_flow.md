graph TD
subgraph Import Data
A[/Payroll Data - Employee Information/]
B[/Payroll Data - GL Codes/]
C[/Payroll Data - Paysheet/]
D[/Payroll Data - Timesheet/]
end
F[(Global setup - Companies - Cost Centers - COA Tables)]
E[(Global Setup - Business Associates)]
G[(EXD Setup - Account Codes)]
H[(Global Setup - EXD Code Table)]
I[(EXD Setup - Pay Codes)]
J[(EXD Setup - Paysheet Translation)]
K[(EXD Setup - Payrun Calendar)]
L[(EXD Results - Paysheet Results)]
M[Paysheet Translation Process]
N[Timesheet Override Process]
O[Employee Rate Calculations Process]
subgraph Expense and Override Process
P[Expense Results Process]
Q[Override Results Process]
end
R[EXD Final Process]
subgraph Import Process
S[Import GL Codes Process]
T[Import Ap Staff Process]
U[Import Timesheet Process]
V[Import Paysheet Process]
end
W[(EXD Results - Timesheet Results)]
subgraph results
X[(EXD Results - Journal Entries Paysheet Translation)]
Y[(EXD Results - Journal Entries Timesheet Override)]
end
Z[(EXD Results - Summarized Journal Entries)]
AA[(Journal Entry)]
A --> T

T --> E
B --> S
S --> E
F --> G
E --> G
H --> G
H --> I
H --> J
I --> J

%% Paysheets
C --> V
V --> L

%% Timesheet
D --> U
U --> W

L --> M
J --> M
K --> M
M --> X
X --> O
O --> N
N --> Y
W --> O

X --> P
Y --> Q

%% Expense and Override to SJE
P --> Z
Q --> Z

%% Final to JE
Z --> R
R --> AA
