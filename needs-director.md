# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given: I have the record of registrations of the patients for all days
  And the calendar mentioned all working days and holidays.
  
  When: I calculate total number of registrations on working days and holidays.
  
  Then: I have the number of patients visit during working days and holidays.
  
Scenario: Compute parking slots to reserve for visiting specialists

  Given: I have data of total number of parking slots
  And the number of parking slots occupied daily for a week.
  
  When: I subtract
  Average number of parking slots occupied daily
  From
  Total number of parking slots.
  
  Then: I have the number of parking slot reserved for visiting specialists.
