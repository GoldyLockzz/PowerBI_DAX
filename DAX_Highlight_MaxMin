Highlight_MaxMin = 
VAR Sales = [Total Sales]
-- Dont forget create QuarterNo and Year Column 1st
VAR MaxSalesOverall = 
        MAXX(
            ALLSELECTED(
                Date_Table[Year],Date_Table[QuarterNo]),[Total Sales]
        )

VAR MinSalesOverall =
        MINX(
                ALLSELECTED(
                    Date_Table[Year],Date_Table[QuarterNo]),[Total Sales]
            )
RETURN
    IF([Total Sales]=MinSalesOverall,"#ff908c",
        IF([Total Sales]=MaxSalesOverall,"#22957e",BLANK())
        )
// VAR Result =
//     SWITCH(
//         TRUE(),
//         Sales = MaxSalesOverall, ,
//         Sales = MinSalesOverall, ,
//         "#7bc8fe"
//     )
// RETURN
//     Result
