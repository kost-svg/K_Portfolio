# K_Portfolio
Example data science portfolio
# Project 1:  Data Science Dock door allocation optimisation & yard performance modeling for trucks and trailers for customer in USA
  * Improve yard efficiency and decrease cost:
- By predicting the yard processing time ( check-in to close-trailler time ) for each trailer, the factory would be able to identify detention candidate trucks and take proactive measures to shorten their yard processing time.
- By listing out the reasons for potential detention of each detention candidate, yard managment will be able to focus on the optimal action to decrease trucks processing time.
- By optimizing the dock door assignemnt, yard process effciency may increase, detention time & detention cost decrease. 
# Ranking Customers by yard priority for customer in USA
   * Analyze if there are certain customers which have yard priority over others, in order to gain perspective about what happens when there are several trailers checking in at the same time. 
   * We define a shipment as prioritised if the shipment has been checked in after another shipment, but has a dock allocated earlier than the other shipment. Meaning that even though the shipment arrived later it received a dock door earlier than the other shipment!
   * The first scoring takes into consideration the Net Priority %, which is the difference between the percentage of shipments which have been prioritised and the percentage of shipments which lost priority by another shipment.  The higher the percentage the higher priority one customer has. After calculating it, the score is min-max normalised,the lower the score, the better. The scores range from 0 to 5.
   * Following the first scoring, we do a second scoring for each customer which is based on the first scoring. Namely, this score is calculated by summing the positive differences in shipments prioritised by a customer which has a lower first score. Meaning that the head to head comparison of customers is taken into account.   
# Effect on problematic inventory on yard performance of other shipments  (HOU,ATL,TAC & MIS). 
   * The data for shipments ranges from 16th of April 2020 to 29th of December 2020
   * For each shipment  at its moment of checking in we calculate the following formula:
  If this equation does not apply to the given shipment we categorize it as a problematic shipment
  This analysis focuses on the shipments which were in CIFL phase while a problematic inventory trailer was checked in. 
  # Customer Pickup
   * The analysis identifies the differences in checking in behaviour of individual Customers that use the CPU option for shipments in different plants.
   * The TTO dataset is used for this analysis from May 2021 to 16 August 2021.
   * Only customers with more than 250 CPU shipments in this period are considered and only carriers with more than 
   * In order to establish the overall earliness/lateness of each shipments, we used the Start Time timestamps, as the closest to the real scheduled appointment time and closest to the Check In Timestamp. 
   * Trailers are considered as “On Time” if they have arrived ± 60 minutes of their Start Time timestamp. 





