# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given A calendar and a sensor which is working
  When patient visits on a working day or holiday
  Then increment the count variable for each category.

Scenario: Compute parking slots to reserve for visiting specialists

  Given Number of available parking slots and count of
  visiting specialists on a day
  When the specialist enters the premises
  Then increment and block the parking slot.
