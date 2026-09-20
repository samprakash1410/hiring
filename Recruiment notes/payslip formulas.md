//formulas to use payslip/

emp name:
 =VLOOKUP(B7,RAW_DATA_TABLE,2,0)

  emp designation:
   =VLOOKUP(B7,RAW_DATA_TABLE,4,0)

    emp bank account numbr:
     =VLOOKUP(B7,RAW_DATA_TABLE,9,0)

      emp bank:
       =VLOOKUP(B7,RAW_DATA_TABLE,6,0)

        emp joing date:
         =VLOOKUP(B7,RAW_DATA_TABLE,3,0)

          emp total working days:
           =VLOOKUP(B7,RAW_DATA_TABLE,13,0)

            emp attend working days:
             =VLOOKUP(B7,RAW_DATA_TABLE,12,0)

              emp month salary:
               =VLOOKUP(B7,RAW_DATA_TABLE,10,0)

                emp basic salary:
                 =VLOOKUP(B7,PAYROLL_TABLE_SHEET,6,0)

                  emp overtime allowance:
                   =VLOOKUP(B7,PAYROLL_TABLE_SHEET,9,0)

                    emp dearness allowance:
                     =VLOOKUP(B7,PAYROLL_TABLE_SHEET,10,0)

                      emp hra:
                       =VLOOKUP(B7,PAYROLL_TABLE_SHEET,11,0)

                        emp ta:
                         =VLOOKUP(B7,PAYROLL_TABLE_SHEET,12,0)

                          emp ia:
                           =VLOOKUP(B7,PAYROLL_TABLE_SHEET,13,0)

                            emp pf:
                             =VLOOKUP(B7,PAYROLL_TABLE_SHEET,15,0)

                              emp pt:
                               =VLOOKUP(B7,PAYROLL_TABLE_SHEET,16,0)

                                emp totoal deductions:
                                 =sum(pt:pf)

///////////////////--------------formulas for the payslip for emp///////////////////////

 formula for payrolland payslip is :
 *=vlookup(b2 means emp id,Table1 data store values,6 for emp name row value,0)* 
        
                                =vlookup(b2,table1,6,0)

       this is one we can make single formula for hole data sheets payroll and paysilp easly we can get easly manner.