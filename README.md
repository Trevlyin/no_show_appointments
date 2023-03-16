# No-show Appointments Analysis

Analysis for Patients in Brazil Medical appointments and centered on the question of whether or not patients show up for their appointment

# Dataset

The Dataset can be obtained from [Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments). It contains 100K records of medical appointments in Brazil and is focused on if patients will show up or not.

It has the following patient charecteristics:

1. PatientId: Identification of a patient
2. AppointmentID: Identification of each appointment
3. Gender: Male or Female.
4. AppointmentDay: The day of the actual appointment, when they have to visit the doctor.
5. ScheduledDay: The day someone called or registered the appointment, this is before appointment of course.
6. Age: How old is the patient.
7. Neighbourhood: Where the appointment takes place.
8. Scholarship: True of False . Observation, on [Bolsa Familia](https://en.wikipedia.org/wiki/Bolsa_Fam%C3%ADlia)
9. Hipertension: True or False
10. Diabetes: True or False
11. Alcoholism: True or False
12. Handcap: True or False
13. SMS_received: 1 or more messages sent to the patient.
14. No-show: True or False.

# Create an environment
To create an environment from an environment file, use the following command:

> conda env create -f environment.yaml

# Summary Findings

Among the selected features, *age*, *gender*, and all diagnostic diseases features(*hipertension, diabetes, alcoholism*) and also patients on the **Bolsa Familia** scholarship, tend to have no significantly dominant diagnosis group with the target *no_show* as they have the same attendance rate like the rest of the population with a a difference between . 

Patients who have received sms messages surprisingly have a higher chance of not showing up for their appointment with ~7% increase compare with the rest of the population while the latter had a no-show rate reduction of 3.49%. Among the 35 out of 81 neighborhoods with atleast 1% patient population, 10 with a lower no-show rate ranged 15.5% - 18.5%.
