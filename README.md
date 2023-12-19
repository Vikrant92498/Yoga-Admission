The frontend of the project is build with React.
Backend : NodeJs + ExpressJs + MySQL(database)
Frontend is deployed on Netlify
Backend is deployed on render

Frontend
When the user open the link https://yogaclassadmission.netlify.app/ , a form will open which ask user to enter few details . 
![image](https://github.com/Vikrant92498/Yoga-Admission/assets/107363759/60d31558-7c22-4c3c-a232-a48ed1faf6ca)

1. Full Name
2. Age
3. Phone No
4. Fees (This field is not editable and have fixed value)
5. Select Batch : There are 4 batches and a id is assigned to each batch like 1,2,3,4.
6. Duration (Start Date and End Date) will be calculated based on the current day date . It satisfy the requirement that user can pay anyday of month but will have to pay the fee of whole month.
7. A submit Button
8. Reponse from the server will be displayed below the button .

To manage the state of component , I have used useState hook .
When the user first render the page
the startDate and endDate of month will be calculated and displayed to user

Some validations are done on client side like name,age and phone number can't be left empty
After the validation , it make a POST request to the server sending name,age,phone,price,todayDate . 


Backend 
Used CORS 

