# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given: We have a running database.
  
  When: We have a program which updates 
  the visit-counter in every 1 minute duration
  In the databse.
  
  Then: We can recover visit-counter across restarts.

Scenario: Reconcile counts if the sensor is offline for a while

  Given
  When
  Then
