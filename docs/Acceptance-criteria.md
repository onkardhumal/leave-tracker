# Acceptance Criteria (Gherkin)

## Apply Leave
Given user is on leave form  
When valid details are entered  
Then request is created with status "PENDING"

---

## Select Dates
Given user selects start date  
When end date is selected  
Then end date must be >= start date  
And system calculates total days  

---

## View Balance
Given user opens form/dashboard  
Then leave balance is visible  

---

## Approve Leave
Given manager views request  
When approve is clicked  
Then status becomes "APPROVED"  

---

## Reject Leave
Given manager views request  
When reject is clicked  
Then status becomes "REJECTED"  

---

## Revoke Leave
Given user has leave request  
When revoke is clicked  
Then:
- If pending → no balance change  
- If approved → balance restored  

---

## Bulk Approval
Given manager selects multiple requests  
When approve is clicked  
Then all are approved  

---

## Calendar View
Given user opens calendar  
Then approved and pending leaves are visible  

---

## Calendar Selection
Given user selects date range from calendar  
Then form opens with pre-filled dates  

---

## Dashboard Employee
Given employee opens dashboard  
Then all leave requests are listed  

---

## Dashboard Manager
Given manager opens dashboard  
Then pending requests are shown  

---

## Conflict Warning
Given overlapping leave exists  
When user selects dates  
Then warning popup is shown  
