# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given a counter sensor that's turned on
  When the patients enters the hospital
  Then count gets incremented in the sensor.

Scenario: Alert when seating capacity is full

  Given the sensor works fine
  When the seating capacity is full
  Then there is an alert in the sensor.
