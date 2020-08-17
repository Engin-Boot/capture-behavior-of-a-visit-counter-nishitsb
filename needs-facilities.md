# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given: Reception has the entries of all visitors visiting daily.
  
  When: I calculate the number of visitors visiting on each day of the week.
  
  Then: I have a report on how visitor visit trends during a week of operation.

Scenario: Alert when seating capacity is full

  Given: Database has the number of visitors in the premises
  For the current instance of time
  And the total seating capacity of the building.
  
  When: If number of visitors in the premises is equal to 
  The total sitting capacity of the building.
  
  Then: It generate a alert for the same.
