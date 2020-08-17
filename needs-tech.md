# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given: We have a running database.
  
  When: We have a program which updates
  the visit-counter in every 1 minute duration
  In the database.
  
  Then: We can recover visit-counter across restarts.

Scenario: Reconcile counts if the sensor is offline for a while

  Given: Sensor should have some internal memory to store the counts.
  
  When: the sensor gets online it stores the counts in the database.
  
  Then: We can reconcile the counts
  Stored in the internal memory of the sensor
  If it goes offline.
