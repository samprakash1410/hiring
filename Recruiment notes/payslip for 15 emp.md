//payroll sheet for 15 emp//

Emp name
  =VLOOKUP([@[EMPLOYEES''S ID]],Data1,5,0)

  Emp gender
    =VLOOKUP([@[EMPLOYEES''S ID]],Data1,6,0)

   Emp marriage status
      =VLOOKUP([@[EMPLOYEES''S ID]],Data1,7,0)

    Emp dept
       =VLOOKUP([@[EMPLOYEES''S ID]],Data1,14,0)

       Emp basic salary
           =VLOOKUP([@[EMPLOYEES''S ID]],Data1,19,0)

            Emp ot minutes
              = 200
               
               Emp no of working days
                 = 26

                  emp attend days
                    = 25

                     Emp earn basic salary
                        =[@[EMPLOYEE''S BASIC SALARY]]/[@[NO OF WORK DAYS ]]*[@[ATTENDANCE WORK DAYS ]]

                         Emp da
                             =VLOOKUP([@[EMPLOYEES''S ID]],Data1,20,0)*[@[EARNED BASIC SALARY]]

                             Emp hra
                                 =VLOOKUP([@[EMPLOYEES''S ID]],Data1,21,0)*([@[EARNED BASIC SALARY]]+[@DA])

                                 Emp ta >8000
                                    =VLOOKUP([@[EMPLOYEES''S ID]],Data1,22,0)

                                    Emp ia > 5000
                                       =VLOOKUP([@[EMPLOYEES''S ID]],Data1,23,0)

                                       Emp ot
                                         =[@[OT (MIN)]]*100

                                           Emp total earning
                                              =SUM([@[EARNED BASIC SALARY]]+[@DA]+[@HRA]+[@TA]+[@IA]+[@OT])

                                              Emp pf 12%
                                                 =VLOOKUP([@[EMPLOYEES''S ID]],Data1,24,0)*[@[EARNED BASIC SALARY]]

                                                 Emp pt 5%
                                                    =VLOOKUP([@[EMPLOYEES''S ID]],Data1,25,0)*[@[TOTAL EARNING]]

                                                    emp total dedution
                                                       =SUM(Data2[@[PF]:[PT]])

                                                       emp net salary
                                                         = total earning -total dedution


++++++++++++++++++++++++this is for emp 15 members all payroll formula's +++++++++++++++++++++++++++++++++



