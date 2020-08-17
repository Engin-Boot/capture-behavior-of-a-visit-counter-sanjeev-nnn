# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given There is a server containing visitor details
  When The server restarts
  Then Recover visitor detail from backup.

Scenario: Reconcile counts if the sensor is offline for a while

  Given Sensor has tendency to go offline
  When Sensor goes offline
  Then Keep a record of every scanned bar codes.
