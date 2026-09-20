//THE 5 STEPS FOR PAYROLL ACCOUNTING IN MICROSOFT EXCEL//

>Set Up Employee Data Columns:
  Create column headers in the first row.
  Include fields for Employee ID, Name, Pay Rate, and Hours Worked.

>>Enter Employee Information:
   Type or import employee details into each respective row.
   Keep basic salary or hourly wage data updated for the current pay period.

>>>Calculate Gross Pay:
     Use formulas to multiply the pay rate by total hours worked.
     Add overtime earnings if applicable using multiplication and addition.
     ex:= (Hours * Rate) + (Overtime_Hours * Overtime_Rate).

>>>>Determine Taxes and Deductions:
       Create columns for income tax and other withholdings.
       Multiply gross pay by the applicable tax percentage.
       ex:= Gross_Pay * Tax_Rate.

>>>>>Compute Net Pay:
          Subtract total deductions and taxes from the gross pay.
          ex: = Gross_Pay - Total_Deductions.


///tools///

>slicer:
   slicers provide clickable on-screen buttons that make reports interactive, visible, and much easier for everyone to use.

>raw data:
  the original, unprocessed set of values and text imported or typed directly into cells before you apply any formatting, formulas, or analysis.

>import STEPS<

 payroll sheet formulas:
   
   emp name formulas:
     =VLOOKUP([@[EMPLOYEES''S ID]],RAW_DATA_TABLE,2,0)

    emp salary:
     =VLOOKUP([@[EMPLOYEES''S ID]],RAW_DATA_TABLE,10,0)

     emp attendance:
      =VLOOKUP([@[EMPLOYEES''S ID]],RAW_DATA_TABLE,12,0)

      emp total working days:
       =VLOOKUP([@[EMPLOYEES''S ID]],RAW_DATA_TABLE,13,0)

      earnings base salary:
       =[@[EMPLOYEE''S BASIC SALARY]]/[@[Total working days]]*[@[ATTENDANCE WORK DAYS ]]

      emp ot hours:
       =VLOOKUP([@[EMPLOYEES''S ID]],RAW_DATA_TABLE,14,0)

       emp ot rate:
        =VLOOKUP([@[EMPLOYEES''S ID]],RAW_DATA_TABLE,15,0)

        emp ot allowance:
         =[@[ OT HOURS ]]*[@[ OT RATE ]]

         emp da:
          =[@[EARNED BASIC SALARY]]*10%

          emp hra:
           =[@[EARNED BASIC SALARY]]*30%+[@[OT ALLOWANCES ]]*30%

          emp ta:
           5000 for all 5 emp

           emp incent allowance:
            about per person

            emp total earnings:
             =[@[EARNED BASIC SALARY]]+[@[OT ALLOWANCES ]]+[@DA]+[@HRA]+[@TA]+[@IA]

            emp pf:
             =[@[EARNED BASIC SALARY]]*12%

            emp pt:
             =[@[TOTAL EARNING]]*15%

            emp total deductions:
             =SUM(PAYROLL_TABLE_SHEET[@[PF]:[PT]])

            emp net profit:
             =[@[TOTAL EARNING]]-[@[TOTAL DEDUCTION]]

*****///***** these are formulas for payroll sheet formulas***///

