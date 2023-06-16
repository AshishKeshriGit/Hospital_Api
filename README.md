# Information about API:

### Theme:

- We’re going to design an API for the doctors of a Hospital which has been allocated by the
  govt for testing and quarantine + well being of COVID-19 patients
- There can be 2 types of Users
- Doctors
- Patients
- Doctors can log in
- Each time a patient visits, the doctor will follow 2 steps
- Register the patient in the app (using phone number, if the patient already exists, just
  return the patient info in the API)
- After the checkup, create a Report
- Patient Report will have the following fields
- Created by doctor
- Status (You can use enums if you want to):
- Can be either of: [Negative, Travelled-Quarantine, Symptoms-Quarantine,
  Positive-Admit]

- Date

# Instructions about SetUp:

First start with downloading the code and and write npm install on code editor, it will install all dependencies on your editor.
You will need a code editor and mongoDB setup on your computer.
We will use postman to check the api is working or not,So download postman on your computer.

1.Now use this **http://localhost:5000/api/v1/doctors/register** route to register doctor in API and add the info as shown in image

![Screenshot (145)](https://github.com/AshishKeshriGit/Hospital_Api/assets/122431023/e80b54ea-0e87-455f-a056-16325957f2e9)

2.Use this **http://localhost:5000/api/v1/doctors/login** to login as a doctor and add info as shown in image

![Screenshot (146)](https://github.com/AshishKeshriGit/Hospital_Api/assets/122431023/69ee6f9e-502f-4e5c-8ff9-ded8e1b01b4c)

3.Use this **http://localhost:5000/api/v1/patients/register** and add the token in authorization area which is recieved in second point

![Screenshot (147)](https://github.com/AshishKeshriGit/Hospital_Api/assets/122431023/b5dd9291-eeef-4d09-b928-b17f0269e299)


4. Use this **http://localhost:5000/api/v1/patients/64542231f98d0016200a9eee/create_report** to create report and add status you can see the types of
   status in report model.

![Screenshot (148)](https://github.com/AshishKeshriGit/Hospital_Api/assets/122431023/4916417c-1c6e-43e3-96f9-f24c906f65c2)

5.Use this **(http://localhost:5000/api/v1/patients/register)** to register patient
![Screenshot (147)](https://github.com/AshishKeshriGit/Hospital_Api/assets/122431023/c67ead72-1cf5-4a2a-ac0c-680793ce013f)


6. Use this **http://localhost:5000/api/v1/patients/64542231f98d0016200a9eee/all_reports** to get all the reports.

![Screenshot (149)](https://github.com/AshishKeshriGit/Hospital_Api/assets/122431023/b307f49a-f2b7-4220-b898-0a2f63f00fde)
