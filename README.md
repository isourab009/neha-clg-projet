# neha-clg-projet

web = read.csv('website-traffic.csv')
# Re-order the factors in this order
day.names = c("Saturday", "Sunday", "Monday", "Tuesday", "Wednesday","Thursday", "Friday" )
days = factor(web$DayOfWeek, level=day.names)
boxplot(web$Visits ~ days)


The box plot shows:
• Much less website traffic on Saturdays and Sundays, especially Sunday which has less spread
than Saturday.
• Visits increase during the weekday, peaking on Wednesday and then dropping down by Friday.
• All week days seem to have about the same level of spread, except Friday, which is more variable.
• This is a website of academic interest, so these trends are expected.
