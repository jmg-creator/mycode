# mycode
This repository contains a Google Script that automatically send a list of emails from a Google sheet named "Listado".

The first row of the sheet are column headers, thus the code only runs from the row number 2. It is assumed the last row is number 50.

The subject and body of each email can be customized in the function enviarCorreo(candidato).
Run the function enviarCorreos() to send the list of emails from the App Script page.

The sheet is formed by the following columns:

A: Name of the student

B: email of the tutor in the company

C: Finish date of the internship

D: Automatic Control cell. 0 by default. Automatically equals 1 when the internship has finished (current date is > C). 
   If D>=1 and E=0, it Increases +1 every time the Script is run, in order to show how many times the email has been sent to an specific mail.

E: Manual control cell: 0 by defailt. Manually set to 1 when the tutor has answered the email.


